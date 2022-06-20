# vue-tsc dts bug

How to reproduce the problem

```bash
$ pnpm run build:dts

> element-plus-dts@1.0.0 build:dts /Users/mario/Project/element-plus-dts
> vue-tsc --declaration --emitDeclarationOnly

src/demo.vue:9:25 - error TS2742: The inferred type of 'default' cannot be named without a reference to '.pnpm/@vue+shared@3.2.37/node_modules/@vue/shared'. This is likely not portable. A type annotation is necessary.

  9 <script setup lang="ts">
                            
 10 import { ref } from 'vue'
    ~~~~~~~~~~~~~~~~~~~~~~~~~
... 
 18 })
    ~~
 19 </script>
    


Found 1 error in src/demo.vue:9

 ELIFECYCLE  Command failed with exit code 1.
```
