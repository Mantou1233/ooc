# 星脈運轉

```s
start spwn code -> 
    intface k3 q then {
        hi: "hi"
    } end

    cls scope (i:G) <G -> k in G v{k}> then
        run val:int ->
            i q val eq 0 ? err("noZero") or val
        end
    endcls

    fn main (argv:string[]) then
        try: scope<k3>(0) or trace(e) endtry
    endfn

    dnd main set main
;
```