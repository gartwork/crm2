# TODOS

1. add test cases around the form validation in the create new project workflow

# Pre-conditions

1. not on corporate network
1. not on VPN
1. no AV
1. disk encryption disabled
1. firewall disabled

# Test Cases (perform on OSX & Windows)

## Test Case 1

**Action**: create a new project

**Expected Result**: new project is created & it becomes the active served project

## Test Case 2

**Action**: preview an active project in the PhoneGap Dev App

**Expected Result**: you can preview the active project in the PhoneGap Dev App

## Test Case 3

**Action**: preview the active project in the Browser

**Expected Result**: you can preview the active project in the Browser

## Test Case 4

**Action**: add (import) existing project

**Expected Result**: added project is appended to the project list area & it becomes the active served project

## Test Case 5

**Action**: edit `index.html` of the active project, modify `<p class="event received">Device is Ready</p>` to `<p class="event received">Device is Ready. TestXX</p>`

**Expected Result**: PhoneGap Dev App should update to display the updated content

## Test Case 6

**Action**: edit `index.html` of the active project, modify `<p class="event received">Device is Ready</p>` to `<p class="event received">Device is Ready. TestXX</p>`

**Expected Result**: Browser should update to display the udpated content

## Test Case 7

**Action**: edit `config.xml` of the active project, modify `<name>test08ab</name>` node or modify `<widget xmlns="http://www.w3.org/ns/widgets" xmlns:gap="http://phonegap.com/ns/1.0" id="com.phonegap.helloworld" version="1.0.1">` version attribute of the `<widget>` node 

**Expected Result**: PhoneGap Desktop App's project listing should update with the updated content

## Test Case 8

**Action**: change active project in the PhoneGap Desktop (by clicking play on another project or by click stop on the current active project & then clicking play on a different project)

**Expected Result**: PhoneGap Dev App should update to the contents of the new active project

## Test Case 9

**Action**: change active project in the PhoneGap Desktop (by clicking play on another project or by click stop on the current active project & then clicking play on a different project)

**Expected Result**: Browser should update to the contents of the new active project

## Test Case 10

**Action**: change port number in the settings

**Expected Result**: reload the PhoneGap Dev App with the new port make sure the active project is displayed

## Test Case 11

**Action**: change port number in the settings

**Expected Result**: reload the Browser with the new port make sure the active project is displayed

## Test Case 12

**Action**: if multiple IP addresses are listed, click on at least one

**Expected Result**: the Browser should launch displaying the contents of the active project

## Test Case 13

**Action**: remove a project from PhoneGap Desktop

**Expected Result**: the project should be removed from PhoneGap Desktop's project listing 