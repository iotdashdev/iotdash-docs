---
description: Kun's progress and plan.
---

# Dev Plan & Progress



| Symbol | Description |
| :--- | :--- |
| 🍳  | Progressing |
| ❗  | High priority |
| 😅 | Low priority |

## Week 10 \(13th - 19th, July\).

* [ ] Documentation for:
  * [x] Install, Set-up, Deploy
  * [x] APIs 
  * [x] Integration guide ❗ ❗
  * [ ] Database Set-up, Access & Deploy ❗
  * [ ] Backend overview
  * [ ] Frontend overview
* [ ] Network diagram 
  * [x] Directed graph with Arrow Head
  * [x] Better Positioning 
  * [ ] Tree-like structure option 🍳
  * [ ] Randomize node positioning option 🍳
  * [ ] Polish data display of hub/device on Network diagram page 🍳

## Week 11 \(20th - 24th, July\)

* [ ] Modify local python script on raspberry-pi to accept http request from cloud ❗
  * [ ] Try this method: [https://stackoverflow.com/questions/7023052/configure-flask-dev-server-to-be-visible-across-the-network](https://stackoverflow.com/questions/7023052/configure-flask-dev-server-to-be-visible-across-the-network)
* [ ] Deploy the system in **Singapore** \(Current DB and backend are hosting at U.S, slow connection\) 😅
* [ ] Security 😅
  * [ ] Add token verification for http request
  * [ ] Limit MongoDB access to only backend hosting address
* [ ] UI Polishment
  * [ ] ~~Polish manage page \(The page to view all hubs and their devices\) ❗~~
  * [x] Hub Page  ❗ ❗ ❗ 
  * [x] Remove device page and add hub page to view all devices of particular hub ❗
  * [ ] Add side panel ❗
  * [x] Add filter for hub, or a search bar
  * [x] Appbar polish =&gt; add icon button with toothtip
  * [x] Add logout 🍳
  * [ ] Beautify pop-up forms  \(Create/Delete/Edit\)
* [x] Responsive table view ❗❗❗❗❗❗ 
  * [x] See reference: [https://react-bootstrap-table.github.io/react-bootstrap-table2/storybook/index.html?selectedKind=Basic%20Table&selectedStory=Exposed%20API&full=0&addons=1&stories=1&panelRight=0&addonPanel=storybook%2Factions%2Factions-panel](https://react-bootstrap-table.github.io/react-bootstrap-table2/storybook/index.html?selectedKind=Basic%20Table&selectedStory=Exposed%20API&full=0&addons=1&stories=1&panelRight=0&addonPanel=storybook%2Factions%2Factions-panel)
  * [x] Filter
  * [x] Expandable/Collapsible row to show hub.devices  
  * [x] Buttons to edit/delete/add hub
  * [x] Buttons to edit/delete/add devices

## Week 12 \(27th - 31th, July\)

* [x] Socket Connection from **browser to local raspberry-pi**\(Hub\)
  * [x] To achieve real time streaming of data without passing through backend cloud
* [ ] Research and demo more data visualization methods/form
  * [ ] More network node diagram
  * [ ] Responsive 2d chart with pop-up card





