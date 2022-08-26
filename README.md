# How to Parse Blockchain Transactions to a Google Drive Folder



<p>In this article, we will analyze bitcoin transactions and learn how to parse RawTX very quickly from the blockchain network to the Google Drive folder, all this will help us better understand how bitcoin transactions work and what all its contents are on the blockchain network.<br>
First, we need to know that all bitcoin transactions are stored in [txid].</p>
<blockquote class="wp-block-quote"><p><strong>txid</strong>&nbsp;&nbsp;is the transaction ID stored on the bitcoin blockchain, RawTX is stored in the form of a double hash.</p></blockquote>
<p>This means that RawTX went through the SHA256 algorithm twice to get the transaction hash that we see on the blockchain.</p>
<p>For example, a transaction with this hash:&nbsp;&nbsp;<a href="https://www.blockchain.com/btc/tx/d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f" target="_blank" rel="noreferrer noopener">d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f</a></p>
<p>Transactions on the bitcoin blockchain are stored in the form of a double hash:</p>
<blockquote class="wp-block-quote"><p><code>SHA256(SHA256(0100000001f2068914e2fea859cacd8df990daf4008f11296b3cb953794051147a265d850a000000008b483045022043784344e1e0cb498c1d73b4cee970fb0f9adf38b7891d0b1310fdb9cbc23929022100a734f4e97a05bd169a9f0eb296fc841fa57f8753db09869f8f6f8cc1232616d4014104d6597d465408e6e11264c116dd98b539740e802dc756d7eb88741696e20dfe7d3588695d2e7ad23cbf0aa056d42afada63036d66a1d9b97070dd6bc0c87ceb0dffffffff0100b864d9450000001976a9142df31a60b02cce392822c9a87198753578ef7de888ac00000000) = d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f</code></p></blockquote>
<p>To get RawTX we just need to enter the transaction id [txid],</p>
<p><a href="https://blockchain.info/rawtx/[txid]?format=hex" target="_blank" rel="noreferrer noopener">https://blockchain.info/rawtx/[txid]?format=hex</a></p>
<p>further we will receive information in HEX format, this is our cherished RawTX.</p>
<p><a href="https://blockchain.info/rawtx/d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f?format=hex" target="_blank" rel="noreferrer noopener">https://blockchain.info/rawtx/d76641afb4d0cc648a2f74db09f86ea264498341c49434a933ba8eef9352ab6f?format=hex</a></p>
<p>but as we know, there can be a lot of transactions [txid] in one Bitcoin Address and this is the main problem, which takes a lot of time to find, loads our PC and takes up a lot of disk space.</p>
<p>To solve this problem, just use&nbsp;&nbsp;<code>API</code>&nbsp;the site&nbsp;&nbsp;<strong><a href="https://chain.so/api/" target="_blank" rel="noreferrer noopener">https://chain.so/api/</a></strong></p>
<p>And so, we specify one Bitcoin Address in the bash script:&nbsp;&nbsp;<code>getrawtx.sh «address»</code>&nbsp;and then we extract the entire previous output hash — all inputs refer to the output&nbsp;<code>(UTXO)</code></p>
<blockquote class="wp-block-quote"><p><strong>The UTXO</strong>&nbsp;&nbsp;is the&nbsp;&nbsp;<em>(unspent transaction output)</em>&nbsp;&nbsp;that will be spent on the new input.&nbsp;<em>The hash value of this is&nbsp;&nbsp;</em><code>UTXO</code><em>&nbsp;stored in reverse order.</em></p></blockquote>
<p>As a result, all unspent transaction output will be stored in a file:&nbsp;<code>«RawTX.json»</code></p>
<p>To get&nbsp;&nbsp;<code>RawTX</code>&nbsp;Bitcoin Addresses, use&nbsp;&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/01BlockchainGoogleDrive/getrawtx.sh" target="_blank" rel="noreferrer noopener">the Bash script: getrawtx.sh</a></strong></p>
<figure class="wp-block-image"><img title="Parsing Blockchain in Google Drive" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/7e4268a3ab7e36fc45020c6b222b7611.png" alt="Parsing Blockchain in Google Drive"><figcaption>Parsing Blockchain in Google Drive</figcaption></figure>
<h3>How to parse to the Google Drive folder?</h3>
<p>To do this, you can use the Terminal for Google Colab&nbsp;&nbsp;<strong><a href="https://github.com/demining/TerminalGoogleColab" target="_blank" rel="noreferrer noopener">[TerminalGoogleColab]</a></strong></p>
<p>Earlier I recorded a video tutorial:&nbsp;&nbsp;<a href="https://www.youtube.com/watch?v=S2D7PI6dK08" target="_blank" rel="noreferrer noopener">“TERMINAL in Google Colab creating all the conveniences for working in GITHUB”</a></p>
<h2>Let’s take a closer look at how the Bash script works: getrawtx.sh</h2>
<figure class="wp-block-image"><img title="Bash script: getrawtx.sh" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/06083301bd4339d46a9a62e3d8bd606c.png" alt="Bash script: getrawtx.sh"><figcaption>Bash script: getrawtx.sh</figcaption></figure>
<p><code>./getrawtx.sh 12ib7dApVFvg82TXKycWBNpN8kFyiAN1dr</code></p>
<p>Bitcoin The address that we specify for the&nbsp;&nbsp;<em>utility command</em>&nbsp;<code>wget</code></p>
<figure class="wp-block-image"><img src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/b687859f62fd52efdfe6b536cf3040be.png" alt="How to Parse Blockchain Transactions to a Google Drive Folder"></figure>
<figure class="wp-block-image"><img title="all content is saved to file: index.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/338b5b10ebb67a28ce79bcabb7ed4925.png" alt="all content is saved to file: index.json"><figcaption>all content is saved to file: index.json</figcaption></figure>
<p><a href="https://chain.so/api/v2/get_tx_spent/BTC/12ib7dApVFvg82TXKycWBNpN8kFyiAN1dr" target="_blank" rel="noreferrer noopener">https://chain.so/api/v2/get_tx_spent/BTC/12ib7dApVFvg82TXKycWBNpN8kFyiAN1dr</a></p>
<figure class="wp-block-image"><img title="The grep utility saves all &quot;txid&quot; transaction IDs into one common index2.json file  " src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/07350525294fb491a864ca1d19c4c0f5.png" alt="The grep utility saves all &quot;txid&quot; transaction IDs into one common index2.json file  "><figcaption>The grep utility saves all transaction IDs «txid» into one common file index2.json</figcaption></figure>
<figure class="wp-block-image"><img title="all content is saved to file: index2.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/b0efa6edbf242f2f6f70bc1cc8b87640.png" alt="all content is saved to file: index2.json"><figcaption>all content is saved to file: index2.json</figcaption></figure>
<figure class="wp-block-image"><img title="Delete index.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/4cb904b7a36460710dd6d51679c8317f.png" alt="Delete index.json"><figcaption>Delete index.json</figcaption></figure>
<figure class="wp-block-image"><img title="Using the sed utility, remove the &quot;txid&quot; prefix and quotes commas" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/395b95c44bc13e60cbc0abb38c38108b.png" alt="Using the sed utility, remove the &quot;txid&quot; prefix and quotes commas"><figcaption>Using the sed utility, remove the «txid» prefix and quotes commas</figcaption></figure>
<figure class="wp-block-image"><img title="Final result in file: index2.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/951b6798689d0b357259abf07e711b5a.png" alt="Final result in file: index2.json"><figcaption>Final result in file: index2.json</figcaption></figure>
<figure class="wp-block-image"><img title="Creating a Python Script Using the Echo Utilities" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/3758565cfb656de3fcc0069574fbd93c.png" alt="Creating a Python Script Using the Echo Utilities"><figcaption>Creating a Python Script Using the Echo Utilities</figcaption></figure>
<figure class="wp-block-image"><img title="Run Python script fileopen.py" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/9f0a0fa556623a5c9e436c0f0c118161.png" alt="Run Python script fileopen.py"><figcaption>Run Python script fileopen.py</figcaption></figure>
<figure class="wp-block-image"><img title="After running the Python script fileopen.py, the Bash script rawscript.sh is created" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/8cf23fc9ce47c1fc907eb723b13c7c23.png" alt="After running the Python script fileopen.py, the Bash script rawscript.sh is created"><figcaption>After running the Python script fileopen.py, the Bash script rawscript.sh is created</figcaption></figure>
<figure class="wp-block-image"><img title="Delete index2.json" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/35af1b20063d6255c73c95b6628cd111.png" alt="Delete index2.json"><figcaption>Delete index2.json</figcaption></figure>
<figure class="wp-block-image"><img title="We get permissions for the Bash script rawscript.sh and successfully run it!" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/e63b090910e9e2e08d47b61d0ceb065c.png" alt="We get permissions for the Bash script rawscript.sh and successfully run it!"><figcaption>We get permissions for the Bash script rawscript.sh and successfully run it!</figcaption></figure>
<figure class="wp-block-image"><img title="Delete scripts fileopen.py // rawscript.sh" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/f03a8d9c2ecb1e3576e388c59bf33374.png" alt="Delete scripts fileopen.py // rawscript.sh"><figcaption>Delete scripts fileopen.py // rawscript.sh</figcaption></figure>
<figure class="wp-block-image"><img title="All transactions are saved in the file: &quot;RawTX.json&quot;" src="./How to Parse Blockchain Transactions to a Google Drive Folder - «CRYPTO DEEP TECH»_files/e91dddbaa475462a42032e3b0f87cbc5.png" alt="All transactions are saved in the file: &quot;RawTX.json&quot;"><figcaption>All transactions are saved in the file: «RawTX.json»</figcaption></figure>
<h2>What advantage do we get as a result:</h2>
<ul>
<li>RawTX parsing is fast and everything is saved in one file in the Google Drive folder</li>
<li>unlike the getrawtransaction command&nbsp;&nbsp;<code>«txid»</code>, in the console&nbsp;&nbsp;<code>Bitcoin Сore</code>&nbsp;we do not need to enter&nbsp;&nbsp;<code>«txid»</code>&nbsp;, just enter Bitcoin Address&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/tree/main/01BlockchainGoogleDrive" target="_blank" rel="noreferrer noopener">getrawtx.sh «address»</a></li>
<li>bash script:&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/tree/main/01BlockchainGoogleDrive" target="_blank" rel="noreferrer noopener">getrawtx.sh</a>&nbsp;&nbsp;through&nbsp;&nbsp;site&nbsp;&nbsp;<a href="https://chain.so/api/" target="_blank" rel="noreferrer noopener">API&nbsp;</a><a href="https://chain.so/api/" target="_blank" rel="noreferrer noopener">https://chain.so/api/</a>&nbsp;&nbsp;finds unspent transaction output&nbsp;<a href="https://chain.so/api/">&nbsp;</a><code>(UTXO)</code></li>
</ul>
<p class="has-vivid-cyan-blue-color has-text-color"><strong>Source code:&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/tree/main/01BlockchainGoogleDrive" target="_blank" rel="noreferrer noopener">https://github.com/demining/CryptoDeepTools/tree/main/01BlockchainGoogleDrive</a></strong></p>
<p class="has-vivid-cyan-blue-color has-text-color"><strong>Telegram:&nbsp;&nbsp;<a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener">https://t.me/cryptodeeptech</a></strong></p>
<p class="has-vivid-cyan-blue-color has-text-color"><strong>Video:&nbsp;&nbsp;<a href="https://youtu.be/ECAPypsmMQs" target="_blank" rel="noreferrer noopener">https://youtu.be/ECAPypsmMQs</a></strong></p>
<p><a href="https://cryptodeeptech.ru/blockchain-google-drive"><strong>Source: https://cryptodeeptech.ru/blockchain-google-drive</strong></a></p>

---


|  | Donation Address |
| --- | --- |
| ♥ __BTC__ | 1Lw2kh9WzCActXSGHxyypGLkqQZfxDpw8v |
| ♥ __ETH__ | 0xaBd66CF90898517573f19184b3297d651f7b90bf |
