# 📄 DocuGen AI
### 〜 文章作成の「0→1」を、AIと共に乗り越えるアシスタント 〜

文章作成における「最初の一歩」の心理的ハードルを下げるための、StreamlitベースのWebアプリです。
単なる文章生成ではなく、ビジネスフレームワークに基づいた論理的な構成案の作成をサポートします。

## 🌟 開発の背景
「白紙の状態から構成を考える（0→1）」作業は、最もエネルギーを消費します。
「構成案さえあれば、執筆はもっとスムーズに進むはず」という実体験に基づき、自分の悩みを解決するために開発しました。

## ✨ 主な機能
- **提案書作成:** PREP法に基づいた論理構成で、相手の「YES」を引き出す草案を作成。
- **報告書作成:** 事実と解釈を分離し、AIによる客観的なリスク分析と対策を提示。
- **設計書作成:** アーキテクチャ案の提示に加え、シニアエンジニア視点での技術選定アドバイス。
- **Word出力:** 生成した文章を .docx 形式で保存でき、そのまま実務に活用可能。

## 🛠 使用技術
- **Language:** Python 3.x
- **Frontend:** Streamlit
- **AI Model:** Google Gemini 2.5 Flash API
- **Libraries:** google-generativeai, python-docx, python-dotenv

## 🚀 セットアップ方法

### 1. インストール
ターミナルで以下のコマンドを実行し、リポジトリのクローンとライブラリのインストールを行います。

git clone https://github.com/[あなたのユーザー名]/docugen-ai.git
cd docugen-ai
python -m venv venv
# Windowsの場合: .\venv\Scripts\activate
# Mac / Linuxの場合: source venv/bin/activate
pip install -r requirements.txt

### 2. 環境変数の設定
プロジェクトのルートフォルダに .env ファイルを作成し、Gemini APIキーを設定してください。

GEMINI_API_KEY=あなたのAPIキーをここに貼り付け

### 3. アプリの起動
以下のコマンドを実行すると、ブラウザでアプリが立ち上がります。

streamlit run app.py

## 💡 こだわったポイント
- **UI/UX:** 「黄緑〜緑」を基調とした清潔感のあるデザインと、直感的に操作できる2カラムレイアウト。
- **プロンプトエンジニアリング:** AIを単なる書記ではなく、ユーザーの意思決定を助ける「相談役」として振る舞わせるための指示（システムプロンプト）を工夫しました。

---
© 2026 Mariko Yamaguchi