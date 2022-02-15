# UnityOpenXRTemplate

This repository contains a Unity Editor template that is configured to support development with Open XR, XR Interaction Toolkit, and Oculus Quest.

I built the template following the instructions provided by Lucas M. Haley in this blog post: [How to create a new Unity template from scratch](https://www.lucashaley.com/how-to-create-a-new-unity-template-from-scratch.html)

This template works on Unity Editor version **2021.2.10f1**. If you are using a different version you should change the content of the [package.json](https://github.com/dotdust/UnityOpenXRTemplate/blob/Latest/package/package.json) file:


```
{

"name": "com.dotdust.template.vr",
"displayName": "OpenXR VR",
"version": "1.0.0",
"type": "template",
"unity": "2021.2",
"description": "OpenXR with Oclus Quest 2 VR template",
"dependencies": {},
"repository": {
	"type": "git",
	"url": "https://github.com/dotdust/UnityOpenXRTemplate.git"
}
}
```

Change the line "unity" to whatever major version your Unity Editor is, repack the package:

```
tar czf com.dotdust.template.vr.tgz package/
```

and place it in the templates directory of your Unity Editor.

The location of the templates folder is:

MacOS:
`/Applications/Unity/Hub/Editor/<VERSION>/Unity.app/Contents/Resources/PackageManager/ProjectTemplates`

Windows:
`\Program Files\Unity\Hub\Editor\<VERSION>\Editor\Data\Resources\PackageManager\ProjectTemplates`

In the [Release](https://github.com/dotdust/UnityOpenXRTemplate/releases) section of this repository, you will find a packaged version of the template ready for use.

Hope this will help. Have fun!
