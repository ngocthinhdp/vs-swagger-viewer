# Swagger Viewer - v2.0.0
**Swagger Viewer lets you preview and validate Swagger 2.0 and OpenAPI files as you type in Visual Studio Code.**

It works on swagger files in json and yaml format. Preview and validation happens in real time as you type.

## Preview

To  start
* Open the swagger file and press F1.
* Run the Command `Preview Swagger`.

OR
* Press  `Shift + Alt + P`

OR
* Right click file in explorer panel and click `Preview Swagger`

THEN

* Preview it in vscode Itself like this

![Swagger Preview](https://cdn.rawgit.com/arjun-g/vs-swagger-viewer/2.0.0/docs/swagger-preview.gif)

![Swagger Context Menu](https://cdn.rawgit.com/arjun-g/vs-swagger-viewer/2.0.0/docs/swagger-context-menu.png)

### Opening In External browser

If you want to preview the changes in external browser change the settings `swaggerViewer.previewInBrowser` to `true`

![Swagger Settings](https://cdn.rawgit.com/arjun-g/vs-swagger-viewer/2.0.0/docs/swagger-settings.png)

THEN
* Run the Command `Preview Swagger`.

OR
* Press  `Shift + Alt + P`

**Preview will be automatically opened in default browser.**

### Change Default Port

Default port of the preview url can be changed by changing the `swaggerViewer.defaultPort` value in `User/Workspace Settings`

## Validation (Partial)

Swagger Viewer validates your documents against Swagger 2.0 and OpenAPI specifications. If there are any issues it will be shown as a warning in the problems panel. Right now only one validation error will be shown even if there are multiple issues.

![Swagger Validation](https://cdn.rawgit.com/arjun-g/vs-swagger-viewer/2.0.0/docs/swagger-validation.png)

## TODO
* Show all the errors during validation
* Add code complete support based on Swagger 2.0 and OpenAPI specifications

## Releases

**v2.0.0 Changes**
* Code base changed to TypeScript
* Partial validation support added
* OpenAPI Support added (Not fully tested)
* Only one server runs for the preview page
* Multiple files can be previewed at a time inside vscode
* Context menu added to the explorer to start the preview directly without opening the file
* Using files from swagger-ui-dist npm package - By [@Raptor399](https://github.com/Raptor399) [https://github.com/arjun-g/vs-swagger-viewer/pull/36](https://github.com/arjun-g/vs-swagger-viewer/pull/36)
* Multiple minor bug fixes

v1.7.0 Changes
* Fixed issue in json file parsing. - By [@Zlass](https://github.com/Zlass) [https://github.com/arjun-g/vs-swagger-viewer/pull/27](https://github.com/arjun-g/vs-swagger-viewer/pull/27)

v1.6.0 Changes
* Added support for .yaml, .yml, .json and unsaved documents. - By [@DW8Reaper](https://github.com/DW8Reaper) [https://github.com/arjun-g/vs-swagger-viewer/pull/21](https://github.com/arjun-g/vs-swagger-viewer/pull/21)

v1.5.0 Changes

* Upgraded Swagger UI v3 for preview. - By [@jienco](https://github.com/jienco) [https://github.com/arjun-g/vs-swagger-viewer/pull/17](https://github.com/arjun-g/vs-swagger-viewer/pull/17)

v1.4.0 Changes

* Fixed - Preview of JSON Swagger files not getting updated in realtime. - By [@tmsns](https://github.com/tmsns)
* Fixed - Preview window in vs code not switching to latest file.
* Added - File name in preview window to identify which file is in preview.
* Some performance fixes

v1.3.0 Changes

* Added - Now preview swagger inside the editor itself. - By [@ferreus](https://github.com/ferreus) [https://github.com/arjun-g/vs-swagger-viewer/pull/7](https://github.com/arjun-g/vs-swagger-viewer/pull/7)
* Added - Preview inside editor by default

v1.2.0 Changes

* Added - `Open` button in message box. - By [@pmentz](https://github.com/pmentz) [https://github.com/arjun-g/vs-swagger-viewer/pull/3](https://github.com/arjun-g/vs-swagger-viewer/pull/3)
* Added - shortcut `Shift + Alt + P` to run the command
* Added - Ability to change default port from `User/Workspace Settings`.

### Credits
Swagger Viewer utilizes the following open source projects
* [Swagger Editor](https://github.com/swagger-api/swagger-editor)
* [Swagger Parser](https://github.com/BigstickCarpet/swagger-parser)
* [Express](https://github.com/expressjs/express)
* [socket.io](https://github.com/socketio/socket.io/)
* [yaml.js](https://github.com/jeremyfa/yaml.js)

### Contributors
* [Patrick Mentz (@pmentz)](https://github.com/pmentz)
* [Vladimir Vainer (@ferreus)](https://github.com/ferreus)
* [Jonatan Ienco (@jienco)](https://github.com/jienco)
* [@tmsns](https://github.com/tmsns)
* [@DW8Reaper](https://github.com/DW8Reaper)
* [@Zlass](https://github.com/Zlass)
* [@Raptor399](https://github.com/Raptor399)