# jspm-ts-bundle
Experimental repo to demonstrate JSPM TS bundling problems. 

1. pull
1. `npm install`
1. `npm run bundle`

```
> ts-bundle@1.0.0 bundle /home/petr/dev/ts-bundle
> jspm bundle 'src/**/* - [src/**/*]' build/built.js

     Building the bundle tree for src/**/* - [src/**/*]...
     
       github:jspm/nodelibs-process@0.1.2
       github:jspm/nodelibs-process@0.1.2/index
       npm:lodash@3.10.1
       npm:lodash@3.10.1/index
       npm:process@0.11.2
       npm:process@0.11.2/browser
       src/boot.ts!github:frankwallis/plugin-typescript@2.4.5
       src/component.ts
       src/component.ts!github:frankwallis/plugin-typescript@2.4.5
     
ok   Built into build/built.js with source maps, unminified.
```

but `src/*` files should not be included...
