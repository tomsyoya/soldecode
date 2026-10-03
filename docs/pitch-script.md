# SolDecode — 1-minute pitch script

**0:00-0:12**

Every Solana team ends up writing their own fragile transaction parser from scratch. It's slow, error-prone, and reinvented on every single project.

> Solanaのチームはどこも、独自の壊れやすいトランザクションパーサーをゼロから書いています。遅くてバグも多く、プロジェクトごとに同じ作業が繰り返されています。

**0:12-0:27**

SolDecode is an open-source Go SDK that decodes raw Solana instructions into clear, structured actions. For example, 'swapped 2 SOL for 150 USDC'.

> SolDecodeはオープンソースのGo製SDKで、Solanaの生の命令を分かりやすい構造化データに変換します。例えば『2 SOLを150 USDCにスワップした』のように表現します。

**0:27-0:42**

Developers send a transaction signature or wallet address through our REST API or CLI. SolDecode fetches the raw data from Solana RPC, finds the right decoder, and returns clean, structured JSON events.

> 開発者はREST APIやCLIを通じてトランザクション署名やウォレットアドレスを送信するだけです。SolDecodeがSolana RPCから生データを取得し、適切なデコーダーを見つけて、整った構造化JSONイベントを返します。

**0:42-0:52**

It already supports System, Token, Jupiter, Orca, and Marinade programs, with a plugin architecture for adding more.

> すでにSystem、Token、Jupiter、Orca、Marinadeといったプログラムに対応しており、プラグイン構造で簡単に拡張できます。

**0:52-1:00**

As non-crypto developers join Solana, shared decoding infrastructure is essential. SolDecode is building that foundation. Thank you.

> 非web3の開発者がSolanaに参入する中、共有のデコード基盤は不可欠です。SolDecodeはその土台を作っています。ありがとうございました。
