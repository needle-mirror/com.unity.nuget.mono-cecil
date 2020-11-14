|  Candidates Repo | Production Repo  |
| ---------- | ------ |
| ![CandidatesBadge](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/candidates-badge.svg) | ![ReleaseBadge](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/release-badge.svg) |

| Release Stream | Status | Build Status | Dependancies | Dependants | Warnings |
| ---------- | ------ | ------ | ------ |  ------ |  ------  |
| 0.1.x [*main*] | Development | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/build-badge.svg?branch=main&testWorkflow=package-isolation)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/build-info?branch=main&testWorkflow=package-isolation) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependencies-badge.svg?branch=main&testWorkflow=updated-dependencies)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependencies-info?branch=main&testWorkflow=updated-dependencies) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependants-badge.svg)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependants-info) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/warnings-badge.svg?branch=main)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/warnings-info?branch=main) |
| 0.1.6-preview [*release/nuget.mono-cecil*] | Archive | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/build-badge.svg?branch=release/nuget.mono-cecil&testWorkflow=package-isolation)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/build-info?branch=release/nuget.mono-cecil&testWorkflow=package-isolation) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependencies-badge.svg?branch=release/nuget.mono-cecil&testWorkflow=updated-dependencies)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependencies-info?branch=release/nuget.mono-cecil&testWorkflow=updated-dependencies) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependants-badge.svg)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependants-info) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/warnings-badge.svg?branch=release/nuget.mono-cecil)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/warnings-info?branch=release/nuget.mono-cecil) |
| 1.0.0-preview.1 [*release/shim*] | LTS - SHIM for Namespace Change | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/build-badge.svg?branch=release/shim&testWorkflow=package-isolation)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/build-info?branch=release/shim&testWorkflow=package-isolation) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependencies-badge.svg?branch=release/shim&testWorkflow=updated-dependencies)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependencies-info?branch=release/shim&testWorkflow=updated-dependencies) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependants-badge.svg)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependants-info) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/warnings-badge.svg?branch=release/shim)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/warnings-info?branch=release/shim) |
| 1.10.0 [*release/mono-0.10.0*] | LTS | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/build-badge.svg?branch=release/mono-0.10.0&testWorkflow=package-isolation)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/build-info?branch=release/mono-0.10.0&testWorkflow=package-isolation) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependencies-badge.svg?branch=release/mono-0.10.0&testWorkflow=updated-dependencies)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependencies-info?branch=release/mono-0.10.0&testWorkflow=updated-dependencies) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependants-badge.svg)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/dependants-info) | [![](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/warnings-badge.svg?branch=release/mono-0.10.0)](https://badges.cds.internal.unity3d.com/packages/nuget.mono-cecil/warnings-info?branch=release/mono-0.10.0) |

# Version

This package wraps the Mono-Cecil DLLs.	This is a **SHIM Package** to change the namespace of the mono-cecil package from `nuget.mono-cecil` to `com.unity.nuget.mono-cecil`

### CI / Yamato
https://yamato.cds.internal.unity3d.com/jobs/1016-com.unity.nuget.mono-cecil

# Using the package

 In the target package, modify the asmdef to include the `Mono.Cecil.dll` under the Assembly References section in the asmdef inspector. The section will not appear until the Override References toggle above is toggled on. Once that is done, your package will have full access to the apis.

 # Add to your project with version

 Open the manifest.json for your project and add the following entry to your list of dependencies with the desired version

 ```json
 "com.unity.nuget.mono-cecil": "0.1.6-preview.3",
 ```

 Example:

 ```json
 {
   "dependencies": {
     "com.unity.nuget.mono-cecil": "0.1.6-preview.3",
     "com.unity.ads": "2.0.8",
     "com.unity.analytics": "3.2.2",
     "com.unity.collab-proxy": "1.2.15",
     ...
     }
  }
  ```

  # Add to your Package as a dependency

  Open the package.json for your projet and add the following entry to the dependencies list with the desired Version

 ```json
 "com.unity.nuget.mono-cecil": "0.1.6-preview.3"
 ```

 Example:
 ```json
  "dependencies": {
 		"com.unity.nuget.mono-cecil": "0.1.6-preview.3"
 	},
 ```

# Contact

 If you need to get a hold of the team, the best entry point is the #devs-mono-cecil-package channel in slack.
