<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE topic SYSTEM "https://resources.jetbrains.com/writerside/1.0/xhtml-entities.dtd">
<topic xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:noNamespaceSchemaLocation="https://resources.jetbrains.com/writerside/1.0/topic.v2.xsd"
       id="Empty-MD-Topic" title="CMS web connection">

    <title>
        CMS web connection
    </title>
    <p>If you want use CMS web, you need change your database without prefix srv1_ or edit code at web in user.php</p>

    <code-block>public function __construct($host, $user, $password)
        {
        $database = new Database();

        $account = $database-&gt;dbConnection($host, &quot;account&quot;, $user, $password);
        $this-&gt;account = $account;

        $player = $database-&gt;dbConnection($host, &quot;player&quot;, $user, $password);
        $this-&gt;player = $player;

        $common = $database-&gt;dbConnection($host, &quot;common&quot;, $user, $password);
        $this-&gt;common = $common;

        $sqlite = $database-&gt;dbConnection(&quot;&quot;, &quot;&quot;, &quot;&quot;, &quot;&quot;, &quot;yes&quot;);
        $this-&gt;sqlite = $sqlite;

        $log = $database-&gt;dbConnection($host, &quot;log&quot;, $user, $password);
        $this-&gt;log = $log;
        }
    </code-block>
    <list>
        <li>account -> srv1_account</li>
        <li>player -> srv1_player</li>
        <li>common -> srv1_common</li>
        <li>log -> srv1_log</li>
    </list>
</topic>
