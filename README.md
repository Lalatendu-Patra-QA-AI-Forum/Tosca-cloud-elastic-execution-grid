# 🌐 Connecting Tricentis Tosca Commander with Tosca Cloud Elastic Execution Grid (E2G)

Elastic Execution Grid (E2G) allows us to run Tosca on-premise tests seamlessly on the Tosca Cloud. As a core component of Tosca Cloud, it enables unattended test runs in parallel across multiple agents. E2G automatically distributes your Execution Lists across all available cloud and team agents simultaneously, dramatically shortening regression cycles and optimizing your delivery pipeline.

---

## 💡 Key Benefits of E2G
* **Zero Local Infrastructure Dependency:** Cloud agents run public web and API tests without requiring local hardware or VM configurations.
* **Hands-Off Agent Maintenance:** Tosca Cloud automatically pushes and installs agent updates in the background, completely relieving your team from manual update cycles.
* **True Resource Elasticity:** E2G dynamically allocates parallel execution streams across multiple agents, shrinking your regression cycles and fitting seamlessly into modern CI/CD pipelines.
* **DEX Configuration Free:** Unlike traditional setups, cloud or team agents don't require you to build or maintain complex configuration files tailored to specific DEX machine characteristics. This keeps framework maintenance footprints incredibly low.

---

## 📋 Pre-requisites
1. A **Tosca Cloud Tenant account** equipped with an execution license to create and provision team/cloud agents.
2. A **Tosca On-Premise workspace** with licenses managed securely via Tricentis Tosca Server.

---

## 🛠️ Step-by-Step Configuration Guide

### 1️⃣ Phase 1: Linking Your Local Workspace to Tosca Cloud
1. Launch **Tosca Commander** and open your designated multi-user workspace.
   <img width="975" height="428" alt="image" src="https://github.com/user-attachments/assets/7f9bc2a7-0091-4cf9-bd23-315c896c0a49" />
2. Provide your **User Name** & **Password** (login credentials) to access the project root.
   <img width="975" height="367" alt="image" src="https://github.com/user-attachments/assets/5ca1ab2e-c2d3-40c1-b0a9-220cac607d52" />
3. Look at the status bar in the bottom-right corner and click the **"Not connected to Tosca Cloud"** hyperlink.
   <img width="975" height="422" alt="image" src="https://github.com/user-attachments/assets/1a2fdc6f-d151-48e3-bcda-925696affc64" />
4. When the Tosca Cloud integration popup appears, click the blue **Connect** button.
   <img width="975" height="480" alt="image" src="https://github.com/user-attachments/assets/02d76398-d1ec-4ac0-97bb-bf9f0f5219ae" />
5. Open your web browser, navigate to your live Tosca Cloud homepage, and copy your specific **Tenant Space URL** (e.g., `://tricentis.com...`).
   <img width="975" height="475" alt="image" src="https://github.com/user-attachments/assets/6d0dc8d5-d272-4ccc-8f4a-c7459fb786a4" />
6. Return to Tosca Commander, paste the string into the **Tosca Cloud URL** box, and click **Next**.
   <img width="975" height="478" alt="image" src="https://github.com/user-attachments/assets/d75467ee-98ee-49b8-9700-0b72dadf16a7" />
The engine will try to connect to Tosca Cloud Tenant Account
<img width="804" height="222" alt="image" src="https://github.com/user-attachments/assets/a0865fcb-b230-44c0-bf4d-8b96a2d02f04" />

7. In the subsequent login screen window, provide your Cloud tenant Username and Password on the authentication prompt and click **Next**.
   <img width="975" height="446" alt="image" src="https://github.com/user-attachments/assets/100a250d-366c-42fe-b500-93a460e67302" />
<img width="975" height="447" alt="image" src="https://github.com/user-attachments/assets/298afb70-6fbb-49cb-a290-49b01a068f48" />
8. Once authenticated, click **Got it** to clear the confirmation checkmark window. The bottom status bar will now display **"Connected to Tosca Cloud"**.
<img width="975" height="465" alt="image" src="https://github.com/user-attachments/assets/9059cdd3-cf92-45b0-8836-93ce3de50831" />
<img width="975" height="478" alt="image" src="https://github.com/user-attachments/assets/70c856a7-c194-4ea5-aaf0-880deda9dace" />
### 2️⃣ Phase 2: Provisioning an Elastic Cloud Agent

9. Navigate back to your browser window for Tosca Cloud, select your active workspace, and select **Integrations** on the left-hand navigation panel.
<img width="975" height="448" alt="image" src="https://github.com/user-attachments/assets/b9b26237-e62f-45c3-97d8-2b2fef5793fc" />
Elastic Execution Grid (E2G) section is displayed. It is a cloud-based execution engine designed to distribute and scale automated tests across virtual machines, local data centers, and the cloud. It helps you to run your Tosca-on-prem tests in your cloud elastic execution grid.
<img width="975" height="465" alt="image" src="https://github.com/user-attachments/assets/f73d1449-202f-4b50-961d-ada23ada5b84" />
10. Before setting up the E2G integration, click on the Tosca hologram on top left to navigate to your particular workspace
<img width="975" height="458" alt="image" src="https://github.com/user-attachments/assets/070e052b-4632-43c0-bdff-b3ac48697abd" />
<img width="975" height="423" alt="image" src="https://github.com/user-attachments/assets/5eae372d-e9da-4615-8d13-ec1e2ab3a650" />
11. Expand the **Run** section and click on **Agents**.
<img width="975" height="433" alt="image" src="https://github.com/user-attachments/assets/12182278-9689-4ffb-968d-3c257b44a448" />
Available and Unavailable agents are displayed
<img width="975" height="401" alt="image" src="https://github.com/user-attachments/assets/f0980c40-916f-4e76-b706-c8b3b2973da1" />
12. Click on the Personal Agent hyperlink to view agent characteristics
<img width="975" height="438" alt="image" src="https://github.com/user-attachments/assets/9750c834-41a2-435d-8a79-12065cbf7070" />
Agent characteristics displayed
<img width="975" height="393" alt="image" src="https://github.com/user-attachments/assets/8f948208-9435-4ce7-841a-689077f2865f" />
13. Click the blue **Add new agent** button located on the top right.
<img width="975" height="392" alt="image" src="https://github.com/user-attachments/assets/a394e74e-0eec-45c1-ab9a-7b9a000fa9cb" />
14. In the configuration wizard, enter a distinct name for your agent (e.g., `Any Name_Cloud`).
<img width="975" height="428" alt="image" src="https://github.com/user-attachments/assets/41d88e52-70c1-41c2-8857-796d03893a2d" />
15. In the Settings segment, toggle **"Keep the display on while agent is running"** and **"Turn on LiveView on the agent"** to **On**, then click **Next**.
<img width="975" height="132" alt="image" src="https://github.com/user-attachments/assets/bc7464c7-b5dc-4e5e-bd8c-4cf34d8d583c" />
16. Enter your target agent characteristics (e.g., Key: `Browser`, Value: `Chrome`), hit Enter, and click **Next**.
<img width="975" height="410" alt="image" src="https://github.com/user-attachments/assets/ffd32ad7-7b2d-42a7-bd83-6f6e31f168f0" />
17. The system will auto-generate your runtime launch statements. Click the **Copy** actions to capture both the **Command Prompt Launch Statement** and the unique **Client Secret**, saving them temporarily into a local notepad file. Click **Done**.
<img width="975" height="430" alt="image" src="https://github.com/user-attachments/assets/db97095c-9584-4e28-a846-804057fc5d26" />
Details copied into notepad to be used later
<img width="975" height="113" alt="image" src="https://github.com/user-attachments/assets/82ccb25d-9237-45cd-ad26-82f5e5cd1265" />
**Please Note**: A unique client secret will get generated in every new session. You need to copy and use the client secret generated in your system

18. Open your local windows **Command Prompt (CMD)**, paste the captured launch statement, and press **Enter**.
<img width="975" height="154" alt="image" src="https://github.com/user-attachments/assets/418b10d2-a3c2-434d-928c-56fd7d0e0b75" />
19. When the **Tricentis Launcher** interface renders on screen, paste your saved **Client Secret** into the field and click **OK**. Your team agent status will change to a green **Connected** badge.
<img width="975" height="338" alt="image" src="https://github.com/user-attachments/assets/7cbd9c97-5fce-480c-afd8-c3ce2b3605c9" />
<img width="975" height="113" alt="image" src="https://github.com/user-attachments/assets/91e6b80a-2a0b-43d3-b333-a450e7ef05dc" />
<img width="975" height="334" alt="image" src="https://github.com/user-attachments/assets/215d0120-951e-493e-9247-730349da98cf" />
<img width="975" height="344" alt="image" src="https://github.com/user-attachments/assets/cbef69a1-abaa-4627-a612-c0c6955fef22" />
On checking back in Tosca Cloud, a Tosca Cloud team agent is created
<img width="975" height="386" alt="image" src="https://github.com/user-attachments/assets/f9b098a8-81a4-4012-8b1d-982d7ab19a31" />
20. Click on the Team Agent created to view its complete characteristics
<img width="975" height="431" alt="image" src="https://github.com/user-attachments/assets/61f5311b-5bf1-4942-bbab-67954722a069" />

### 3️⃣ Phase 3: Synchronizing Tosca Server Environment Configurations
21. Open a browser tab, navigate to your local **Tricentis Tosca Server Console** dashboard, and click into **Settings**.
<img width="975" height="409" alt="image" src="https://github.com/user-attachments/assets/309fb932-eb5c-445b-bbc4-f4540dcce654" />
<img width="975" height="388" alt="image" src="https://github.com/user-attachments/assets/2c4a65f7-cf04-410d-88f8-2ec3d5603c96" />
22. Select **Automation Object Service** from the left-hand configuration tree.
<img width="975" height="401" alt="image" src="https://github.com/user-attachments/assets/3f6844ed-ae6b-4525-becf-5b69fcdecf4c" />
<img width="975" height="445" alt="image" src="https://github.com/user-attachments/assets/137334ad-cadb-4be6-bc7d-268397e44339" />
23. Scroll down to the **Execution Environments** section.

24. Toggle the **Distributed Execution** switch to **On** and verify your local Distribution Server Address.
<img width="975" height="408" alt="image" src="https://github.com/user-attachments/assets/a63e619b-31a2-4614-8a27-1a89a089fc17" />
25. Locate the **Elastic Execution Grid** section and toggle the switch to **On**.
<img width="975" height="409" alt="image" src="https://github.com/user-attachments/assets/ba6b1b6b-6ad5-4f72-91e6-5560bf1f3da3" />
<img width="975" height="431" alt="image" src="https://github.com/user-attachments/assets/1d7250a4-a6b6-4c2a-9252-a38383183208" />
26. Navigate back to Tosca Cloud and click on Integrations
<img width="975" height="414" alt="image" src="https://github.com/user-attachments/assets/0906c688-9c29-4f97-a9e0-f2e4bd7c8d73" />
27. Click on Set up Integration button of Elastic execution grid section
<img width="975" height="346" alt="image" src="https://github.com/user-attachments/assets/74e22630-79f0-4bbe-851d-e24102c3e3f8" />
In the subsequent window, select your respective work space
<img width="975" height="416" alt="image" src="https://github.com/user-attachments/assets/eebbe57c-b0af-48db-b88c-3cb50faf0762" />
28. Copy the Tosca Cloud URL, Client ID, Client secret
<img width="975" height="405" alt="image" src="https://github.com/user-attachments/assets/f7bf137b-ebdb-4f7d-8a48-e32ee6c67a12" />
<img width="975" height="158" alt="image" src="https://github.com/user-attachments/assets/42c39442-7587-42ee-9b4b-8d87a6eb9dd8" />
29. Paste your live **Tosca Cloud URL**, **Client ID** (`Tosca_Server`), and the **Client Secret** copied directly from your Cloud integration setup panel. Click **Save** and wait for the services to safely restart.
<img width="975" height="379" alt="image" src="https://github.com/user-attachments/assets/1b3f1201-b8dc-490a-8c32-f7d95b9c4356" />
<img width="975" height="368" alt="image" src="https://github.com/user-attachments/assets/15b608c3-8f6e-4717-b7f0-6696a4fa88ed" />
<img width="975" height="356" alt="image" src="https://github.com/user-attachments/assets/12f9e2ae-e39d-4d5b-9721-f0f2f3c96d7f" />
<img width="975" height="425" alt="image" src="https://github.com/user-attachments/assets/f4e0158b-b950-4a17-abf2-c016ab67d48b" />
Copy the particular workspace id
<img width="975" height="354" alt="image" src="https://github.com/user-attachments/assets/c136e5ea-03cf-4d73-a236-8f6f42d892af" />
30. Come back to Tosca Commander and log into your particular workspace. If you have already logged in as per Step 1 & 2, then skip this step
<img width="975" height="397" alt="image" src="https://github.com/user-attachments/assets/a785dfb8-5c26-46b8-8294-2809c4187763" />
<img width="975" height="342" alt="image" src="https://github.com/user-attachments/assets/8543b1e2-14d3-4a0d-97de-bb698f68bc95" />
31. In Tosca Commander, navigate to `Project -> Settings -> Commander -> DistributedExecution -> ElasticExecutionGrid`.
<img width="975" height="407" alt="image" src="https://github.com/user-attachments/assets/3eb578b0-ac84-4e10-8c22-36b6307c4500" />
<img width="975" height="372" alt="image" src="https://github.com/user-attachments/assets/dda04bd1-160c-40ce-b54c-f90d786f7344" />
<img width="975" height="426" alt="image" src="https://github.com/user-attachments/assets/e9374e0a-0647-4753-a9bc-9bfc2450ba58" />
<img width="975" height="310" alt="image" src="https://github.com/user-attachments/assets/d9e4d719-eab9-49be-8de7-97a91c382fc8" />

32. Ensure the Tosca Cloud URL & Client ID which are available in Tosca Cloud the same details are added in corresponding section in Tosca Commander section
<img width="975" height="405" alt="image" src="https://github.com/user-attachments/assets/b0f06a52-230b-4d7f-a28d-aa01444412f7" />
<img width="975" height="348" alt="image" src="https://github.com/user-attachments/assets/08b2ee33-36a6-4fe3-b340-a85d0dceaf8c" />
### 4️⃣ Phase 4: Setting up Grid Events and Triggering Runs

33. Navigate to your root **Execution** folder in Tosca Commander, check it out, right-click it, and select **Create ElasticExecutionGridEvents folder**.
<img width="975" height="434" alt="image" src="https://github.com/user-attachments/assets/f5ff4646-1267-4ca8-9736-038530e18de2" />
<img width="975" height="431" alt="image" src="https://github.com/user-attachments/assets/83b9429a-1843-4cf0-9ec7-fbcf67b0a402" />
<img width="975" height="402" alt="image" src="https://github.com/user-attachments/assets/6ebf5d14-f697-4495-8933-aee7dd65b7a0" />
34. Right-click your new folder, select **Create ElasticExecutionGridEvent**, and provide a functional descriptive name (e.g., `Demo_Web_Shop_Event`).
<img width="975" height="403" alt="image" src="https://github.com/user-attachments/assets/52776470-fc61-4cd9-9b2e-bef93ebb2cbc" />
<img width="975" height="406" alt="image" src="https://github.com/user-attachments/assets/c69d9f77-3572-408e-9171-fef77c9d492d" />
<img width="975" height="375" alt="image" src="https://github.com/user-attachments/assets/67897acf-f608-4c14-99e4-91f8556949c3" />
<img width="975" height="434" alt="image" src="https://github.com/user-attachments/assets/82987e21-9933-4b9a-9205-3c4543691c92" />
35. Drag your verified target **Execution List** and drop it directly inside this newly created Event.
<img width="975" height="456" alt="image" src="https://github.com/user-attachments/assets/2c75bb1f-fd2b-4a5e-8b47-b7c5bf5eee5b" />
36. Check out the Grid Event, go to its **Properties** pane, and input your cloud parameters:
    * **CloudWorkspaceId:** `default`
    * **AgentCharacteristics:** `CloudAgent;AgentIdentifier=[Your_Agent_Name]-Cloud` *(It’s the same AgentIdentifier name of the cloud agent which you had created previously)
<img width="975" height="435" alt="image" src="https://github.com/user-attachments/assets/896602f7-d8ba-4019-9202-ff240fc282f1" />
You can club multiple agent characteristics together separated by semicolon ; . Ensure there are no blank spaces or trailing spaces around the semicolon
<img width="975" height="456" alt="image" src="https://github.com/user-attachments/assets/aafbc99e-59fe-4b13-97d9-a0b1e02aab4d" />

37. Run a **Check In All** and an **Update All** to commit your framework adjustments.
<img width="975" height="423" alt="image" src="https://github.com/user-attachments/assets/fd8d2eb8-9bcd-428e-95ae-1f761657024a" />
38. Right-click your configured Elastic Execution Grid Event and click **Execute in Tosca Cloud**.
<img width="975" height="402" alt="image" src="https://github.com/user-attachments/assets/47026060-cba3-48e1-a232-05ea6cc1bf03" />
39. Test Execution in Progress
<img width="975" height="398" alt="image" src="https://github.com/user-attachments/assets/09e560f9-4039-4c2d-a509-11cc0edc85a6" />
**Please Note**: Once you click on Execute in Tosca Cloud, the actual execution starts with few seconds’ delay.
---

## 📊 Monitoring Test Runs & Downloading Execution Artifacts
40. **Live Progress Tracking:** Once execution is completed,open your Tosca Cloud Tenant browser tab, expand **Run**,
<img width="975" height="461" alt="image" src="https://github.com/user-attachments/assets/e918e374-0742-4e3d-8687-987fd42937ae" />
*  and click on **Test Runs** to monitor real-time parallel execution streams across your cloud agents.
<img width="975" height="444" alt="image" src="https://github.com/user-attachments/assets/77b2d439-e1af-488a-be2b-d6112fa3b215" />
41.	We can view the Test Event run details in the list of Test Runs. Test Event ran in Tosca Cloud through Tricentis Team Agent
<img width="975" height="445" alt="image" src="https://github.com/user-attachments/assets/9fe0162e-2afb-474b-ae86-972a9012d928" />
42. **In-Depth Execution Logs:** Click into a specific target run log to analyze step durations, verification statuses, and download full execution runtime text files.
<img width="975" height="454" alt="image" src="https://github.com/user-attachments/assets/b3477afb-1e2b-4695-bc75-fb491a3cf43b" />
<img width="975" height="443" alt="image" src="https://github.com/user-attachments/assets/643af832-dc6e-4e2d-bdd1-2bf0d3d66bb8" />
43.	Expand the execution list to view details
<img width="975" height="415" alt="image" src="https://github.com/user-attachments/assets/3386c8ea-75ae-486e-81cc-9620c60e032d" />
Execution Details are displayed
<img width="975" height="423" alt="image" src="https://github.com/user-attachments/assets/b1a1b7bc-fd0b-4d11-a6cc-056f6fe9e20a" />
44. Click on each test step folder to view the test execution status of each test step
<img width="975" height="435" alt="image" src="https://github.com/user-attachments/assets/fdbc7de1-9790-4efb-a58c-aff8fa5f2208" />
Click on the ribbon to keep only the central section on the forefront
<img width="975" height="349" alt="image" src="https://github.com/user-attachments/assets/d2efa243-6a51-4a82-8aeb-ced1e2484e3c" />
<img width="975" height="468" alt="image" src="https://github.com/user-attachments/assets/b0d75ab0-611f-47de-bb40-e62e56e86f7b" />
45. Click on Agent Info tab to view Agent details through which execution list of Tosca Commander got executed in Tosca Cloud through elastic-to-grid (E2G) principle
<img width="975" height="419" alt="image" src="https://github.com/user-attachments/assets/f3ea8432-8c7a-409a-8313-f07e34894ba1" />
46. Click on Logs to view the Execution Log details. The log can be downloaded as well through the download icon
<img width="975" height="427" alt="image" src="https://github.com/user-attachments/assets/ad2874b3-279f-4a11-b8ad-41430cdccfb7" />
47. Click on Recording tab to view any recordings generated
<img width="975" height="375" alt="image" src="https://github.com/user-attachments/assets/80b63c7b-b313-4e72-b665-1d6626b608dc" />
**Please Note**: Recordings are only generated for failed test execution runs.
<img width="975" height="393" alt="image" src="https://github.com/user-attachments/assets/f24e36b7-90f2-4bcf-bf78-04ef68ae05df" />
<img width="975" height="442" alt="image" src="https://github.com/user-attachments/assets/69f78a48-ad13-433d-9294-3c2a04c44fbd" />
<img width="975" height="426" alt="image" src="https://github.com/user-attachments/assets/c6d65ca1-501e-4bed-864f-e8d642640b75" />
* **Video Screen Recordings:** If a test case encounters an execution exception or failure state, navigate to the **Recording** tab to review real-time UI video playbacks.
<img width="975" height="472" alt="image" src="https://github.com/user-attachments/assets/e90a7292-ee7b-4c80-91f3-663641170b06" />
* **Attachment Retrieval:** Go to the **Attachments** pane to instantly download consolidated summary logs, including `logs.txt`, `TestSteps.json`, `TBoxResults.tas`, and standard XML test reports.
<img width="975" height="386" alt="image" src="https://github.com/user-attachments/assets/32c70545-3496-410a-8a21-6a346a572ba9" />
48. Come back to Tosca Commander and navigate to the original execution list. Expand the execution list to view the execution details of all the runs done on Tosca Cloud
<img width="975" height="430" alt="image" src="https://github.com/user-attachments/assets/43731236-9a16-49d2-9346-c78674598c43" />
<img width="975" height="407" alt="image" src="https://github.com/user-attachments/assets/4da2eb2b-0a34-4b5a-abfd-5bff41bcc8cb" />

---

## 🎨 INFROGRAPHIC BLUEPRINT FLOW
<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/fbc43856-86cd-4bae-b9ae-7b2d2ce012ad" />
<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/03af2bd7-3f51-4f7d-ac7a-3e66387b73af" />
