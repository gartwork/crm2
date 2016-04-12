### Pre-conditions

1. not on corporate network
1. not on VPN
1. no AV
1. disk encryption disabled
1. firewall disabled

### Test Cases

1. create a new project: new project is created & it becomes the active served project
1. make sure you can preview the active project in the PhoneGap Dev App
1. make sure you can preview the active project in the Browser
1. add (import) existing project: added project is appended to the project list area & it becomes the active served project
1. edit `index.html` of the active project, modify `<p class="event received">Device is Ready</p>` to `<p class="event received">Device is Ready. TestXX</p>`
  - PhoneGap Dev App should update to display the updated content
  - Browser should update to display the udpated content
1. edit `config.xml` of the active project, modify `<name>test08ab</name>` node or modify `<widget xmlns="http://www.w3.org/ns/widgets" xmlns:gap="http://phonegap.com/ns/1.0" id="com.phonegap.helloworld" version="1.0.1">` version attribute of the `<widget>` node - PhoneGap Desktop App's project listing should update with the updated content
1. change active project in the PhoneGap Desktop (by clicking play on another project or by click stop on the current active project & then clicking play on a different project)
  - PhoneGap Dev App should update to the contents of the new active project
  - Browser should update to the contents of the new active project
1. change port number in the settings
  - reload the PhoneGap Dev App with the new port make sure the active project is displayed
  - reload the Browser with the new port make sure the active project is displayed
1. if multiple IP addresses are listed, click on at least one - the Browser should launch displaying the contents of the active project
1. remove a project from PhoneGap Desktop - the project should be removed from PhoneGap Desktop's project listing 
