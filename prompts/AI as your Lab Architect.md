# AI as your Lab Architect

**[C - Character]** "You are an expert Cisco network engineer and {lab_role}."

**[S - Situation]** "I am a {exam_name} candidate, and I am building a hands-on discovery lab to practice for the exam using the blueprint located here: {blueprint_url}"

**[O - Outcome]** "Your goal is to create a fully functional, hands-on CML lab that is based on the blueprint and gives me enough information to complete the task without giving away the answers."

**[P - Purpose]** "I want to practice real exam scenarios in a structured lab environment so I can build confidence and hands-on skills before my exam."

**[E - Example]** "Here are the steps I want you to take:
1. Create a hands-on lab task based on the blueprint, focused on: {lab_focus}.
2. Only have at most **one** related task. Provide enough information to complete the task without giving away the answers.
3. Create a new CML lab and provide the instructions for what I need to perform as lab notes. Lab notes can use markdown for richer text.
4. Create the lab topology in CML using CML Free version, with a maximum of {max_nodes} nodes. Use {lab_nodes}. Unmanaged switches and external connectors do not count toward the maximum. Do not create the full topology right away.
5. First, create an empty lab with the notes, then add the nodes, and then connect them (so the interfaces are right).
6. Update the lab notes with the new, correct interface names.
7. Once the nodes are connected, configure them with any base configuration required for the lab task, using the correct interfaces. Use clearly labeled lab-only placeholder credentials and tell me where to set my own; never reuse real credentials.
8. When complete, start the lab.

Start with **Step 1** to **Step 4**, then wait for my instructions to proceed.
Next, do **Step 5** to **Step 8**."

> This prompt needs an AI assistant connected to CML (for example through a CML MCP server) to build and start the lab. Without it, the AI can still write the task, topology, and lab notes for you to build by hand.
>
> For the CCNA (200-301) exam, set `lab_nodes` to: "only IOL, IOL-L2, ASAv, Desktop, Server, unmanaged switches, and external connectors. Do NOT use IOSv or IOSv-L2."
