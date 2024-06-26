# ⚙️ Web Usage

## MelodyMine Web Developer mode

Running MelodyMine on localhost for developing parts of the website.

{% hint style="warning" %}
Before you start, you need a `MySQL` database.\
\
You can use [XAMPP](https://www.apachefriends.org/) to install `MySQL`. Download and install XAMPP from the link below, then create a database for your server after installation.
{% endhint %}

{% hint style="warning" %}
You also need to have [Node.js](https://nodejs.org) installed on your system. If it's not installed, download and install Node.js.
{% endhint %}

***

### Step 1: **Download Repository**

Download the [MelodyMine](https://github.com/Vallerian/MelodyMine) repository from GitHub.

[https://github.com/Vallerian/MelodyMine](https://github.com/Vallerian/MelodyMine)

***

### Step 2: **Create `.env` file for WebSocket Server**

Navigate to the `web/server` directory and create a file named `.env` with the following values.

```xml
DATABASE_URL="mysql://root:@localhost:3306/melody"
PORT=4000

WEBSOCKET_PLUGIN_AUTH_KEY=random
WEBSOCKET_WEB_AUTH_KEY=random
```

{% hint style="warning" %}
Please note that the `WEBSOCKET_PLUGIN_AUTH_KEY` must match the `plugin_key` in the plugin's `settings.yml` file.\
\
and also, the `WEBSOCKET_WEB_AUTH_KEY` must match the `WEBSOCKET_KEY` in the client's `.env` file.
{% endhint %}

***

### Step 3:  Install Dependency, Prisma and **Run WebSocket Server**

Open a terminal in the `web/server` directory and run the following command.

<pre class="language-bash"><code class="lang-bash"><strong>npm i
</strong>npx prisma generate
<strong>npm run start
</strong></code></pre>

{% hint style="info" %}
Note: Open your browser and ensure that the address `localhost:4000` loads completely.
{% endhint %}

***

### **Step 4: Create `.env` file for Client**

Navigate to the `web/client` directory and create a file named `.env` with the following values.

```markdown
DATABASE_URL=mysql://root:@localhost:3306/melody

NEXTAUTH_SECRET=random 
NEXTAUTH_URL=http://localhost:3000

WEBSOCKET_KEY=random
WEBSOCKET_URL=ws://localhost:4000

TURN_URL=turn:melodymine.taher7.ir:3477
TURN_USERNAME=melodymine
TURN_PASSWORD=melodymine
```

{% hint style="warning" %}
Please note that the `WEBSOCKET_KEY` in the server's `.env` file must match the `WEBSOCKET_WEB_AUTH_KEY`.
{% endhint %}

***

### **Step 5: Install** Dependency, Prisma and **Run Client**

Open a terminal in the `web/client` directory and run the following command.

```bash
npm i
npx prisma generate
npm run dev
```

{% hint style="warning" %}
If you don't want to use Next.js in developer mode, instead of running

```bash
npm run dev
```

use

```bash
npm run build
npm start
```
{% endhint %}

{% hint style="info" %}
Note: Open your browser and ensure that the address `localhost:3000` loads completely.
{% endhint %}

***

### **Step 6:  Download and Install Plugin**

Download the latest version of the MelodyMine plugin from the following link and place it in the `plugins` folder of your server.

[https://github.com/Vallerian/MelodyMine/releases](https://github.com/Vallerian/MelodyMine/releases)

***

### **Step 7: Configure `mysql.yml` file**

Restart the server to generate the plugin files. After the files are created, navigate to the `server/plugins/MelodyMine` directory,

&#x20;open the `mysql.yml` file, and enter your database details.

***

### **Step 8: Configure `settings.yml` file**

Navigate to the `server/plugins/MelodyMine` directory and open the `settings.yml` file.&#x20;

Set the `plugin_key` value to exactly the same value you set in the server's `.env` file for `WEBSOCKET_PLUGIN_AUTH_KEY`:

```xml
WEBSOCKET_PLUGIN_AUTH_KEY=plugin_key
```

***

### **Step 9: Test MelodyMine in Server**

Restart the server to apply the changes. After the server restarts, enter the server and run the command `/melodymine start link`.&#x20;

After receiving the link, click on it to enter the voice chat.

***

{% hint style="info" %}
**If you encounter any issues during the MelodyMine installation, feel free to join the Discord support channel and seek assistance** [**Discord**](https://discord.gg/CBua8YectX)**.**
{% endhint %}
