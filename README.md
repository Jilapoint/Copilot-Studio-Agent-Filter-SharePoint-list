📋 Overview

This is a Microsoft Copilot Studio agent that connects to a SharePoint list to retrieve and analyze inventory data — for example, checking how many devices of a certain type are available.

This agent demonstrates how to combine Copilot Studio Topics, SharePoint connectors, and custom expressions to deliver conversational insights over enterprise data — without writing code or using Power Automate.

🚀 Features

🔗 Connects directly to a SharePoint list (via native connector)

💬 Answers natural-language questions like:

“How many laptops are available?”

“I need a Laptop”

⚙️ Uses built-in Get items connector

🧮 Computes either:

The number of matching records

And the list of matching records

📊 Supports filters with dynamic OData queries

🔐 Works securely under the connected user’s context
🏗️ Prerequisites

Microsoft Copilot Studio access

SharePoint site with a list (e.g., Devices)
Column	Type	Description
| Column   | Type                | Description                         |
| -------- | ------------------- | ----------------------------------- |
| Title    | Single line of text | Device name                         |
| AssetType  | Choice/Text       | Device type (Laptop, Monitor, etc.) |
| Status |    Choice/Text        | Status (Available, Reserved)        |

⚙️ Setup Steps
1️⃣ Import or deploy the Copilot

In Copilot Studio, go to Settings → Import agent.

Choose the exported .zip file from this repository.

Open the imported agent and verify the SharePoint connection.

2️⃣ Configure the SharePoint connection

Edit the Get items connector inside the Available devices topic.

Set:

Site address = your SharePoint site URL

List name = the name of your list (e.g., Devices)

3️⃣ Test the topic

Trigger phrases:

“How many devices do we have?”

“How many laptops are available?”

“List all tablets.”
