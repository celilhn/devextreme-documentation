---
id: dxFileManager.Options.notifications.showPopup
type: Boolean
default: true
---
---
##### shortDescription
Specifies whether to show the pop-up notification window.

---

![DevExtreme File Manager - Show and Hide Popup Notification Panel](/images/FileManager/notifications-popup.png)

---

##### jQuery 

    <!--JavaScript-->
    $(function () {
        $("#file-manager").dxFileManager({
            notifications: {
                showPopup: false
            }
            //...            
        });
    });  

##### Angular

    <!--HTML--> 
    <dx-file-manager id="fileManager">
        <dxo-notifications [showPopup]="false">
        </dxo-notifications>
        <!-- ... -->
    </dx-file-manager>

    <!--TypeScript-->
    import { DxFileManagerModule } from "devextreme-angular";
    // ...
    export class AppComponent {
        // ...
    }
    @NgModule({
        imports: [
            // ...
            DxFileManagerModule
        ],
        // ...
    })

##### Vue

    <!-- tab: App.vue -->
    <template>
        <DxFileManager>   
            <DxNotifications 
                :show-popup="false"
            />
        </DxFileManager>
    </template>
    
    <script>
    import 'devextreme/dist/css/dx.light.css';
    
    import { DxFileManager, DxNotifications } from 'devextreme-vue/file-manager';
    
    export default {
        components: {
            DxFileManager,
            DxNotifications
        },
        data() {
            return {
                // ...
            }
        }
    }
    </script>

##### React

    <!-- tab: App.js -->
    import React from 'react';
    import FileManager, { Notifications } from 'devextreme-react/file-manager';

    const App = () => {
        return (
            <FileManager>
                <Notifications showPopup={false} />
            </FileManager>
        );
    };

    export default App;

##### ASP.NET MVC Controls

    <!--Razor C#-->
    @(Html.DevExtreme().FileManager()
        .Notifications(nt => nt
            .ShowPopup(false)
        )
        // ...
    )

---
