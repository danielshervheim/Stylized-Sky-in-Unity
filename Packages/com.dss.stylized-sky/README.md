# unity-stylized-sky

A procedural stylized skybox shader for Unity.

![all](https://imgur.com/XEnwY1X.png)

See them all in more detail [here](https://imgur.com/a/aB5B7Zz).

## 1. How To Install

The stylized-sky package uses the [scoped registry](https://docs.unity3d.com/Manual/upm-scoped.html) feature to import
dependent packages. Please add the following sections to the package manifest
file (`Packages/manifest.json`).

To the `scopedRegistries` section:

```
{
  "name": "DSS",
  "url": "https://registry.npmjs.com",
  "scopes": [ "com.dss" ]
}
```

To the `dependencies` section:

```
"com.dss.stylized-sky": "1.0.0"
```

After changes, the manifest file should look like below:

```
{
  "scopedRegistries": [
    {
      "name": "DSS",
      "url": "https://registry.npmjs.com",
      "scopes": [ "com.dss" ]
    }
  ],
  "dependencies": {
    "com.dss.stylized-sky": "1.0.0",
    ...
```

## 2. How To Use

- Open the light settings window (`Window > Rendering > Lighting Settings`).
- Drag any of the stylized sky materials from `Packages/Stylized Sky/Runtime/Materials` into the "Skybox Material" slot under the "Environment" dropdown.

## 3. Compatability

Tested on Unity 2019.4 LTS in the standard (SRP) and universal (URP) render pipelines.

## 4. Options

**Sun Disc**
![sun disc](https://imgur.com/ypSPybi.png)

**Sun Halo**
![sun halo](https://imgur.com/fEhTnFO.png)

**Horizon Line**
![horizon line](https://imgur.com/bdgcKMG.png)

**Sky Gradient**
![sky gradient](https://imgur.com/O9nVMrW.png)
