<h1>Peer-to-Peer Encrypted Communication System</h1>

   <div class="section">
        <h2>Summary</h2>
        <p>This Java-based system simulates <strong>secure peer-to-peer communication</strong> using <strong>AES encryption</strong>. It includes two programs:</p>
        <ul>
            <li><strong>Peer:</strong> Can send and receive encrypted messages.</li>
            <li><strong>Receiver:</strong> Only receives and decrypts messages.</li>
        </ul>
    </div>

  <div class="section">
        <h2>How It Works</h2>
        <ol>
            <li><strong>Receiver</strong> listens on port <code>5000</code> and waits for connections.</li>
            <li><strong>Peer</strong> takes user input, encrypts it using AES, and sends it to the specified IP and port.</li>
            <li>Receiver decrypts the incoming message and prints the original text.</li>
        </ol>
    </div>
    <div class="section">
        <h2>Message Transfer Between Two PCs</h2>
        <p>Messages are transferred through a direct socket connection:</p>
        <ul>
            <li>User enters a message, receiver's <strong>IP address</strong>, and <strong>port</strong>.</li>
            <li>Peer encrypts and sends the message over a socket.</li>
            <li>Receiver decrypts the message using the same secret key.</li>
        </ul>
    </div>
    <div class="section">
        <h2>Pros</h2>
        <ul>
            <li>✅ <strong>End-to-End Encryption:</strong> Ensures privacy with AES.</li>
            <li>✅ <strong>No Central Server:</strong> Peer-to-peer model.</li>
            <li>✅ <strong>Simple and Effective:</strong> Easy to understand and extend.</li>
            <li>✅ <strong>Customizable:</strong> Can be expanded with features like GUIs or file sharing.</li>
        </ul>
    </div>
    <div class="section">
        <h2>Cons</h2>
        <ul>
            <li>❌ <strong>Requires Both Peers Online:</strong> No message if receiver is offline.</li>
            <li>❌ <strong>Hardcoded Key:</strong> Not secure for real deployment.</li>
            <li>❌ <strong>No Message History:</strong> Lacks message logging.</li>
            <li>❌ <strong>Firewall/NAT Issues:</strong> Direct connections may be blocked.</li>
        </ul>
    </div>
