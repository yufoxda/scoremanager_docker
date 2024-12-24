# ベースイメージとして Node.js を使用
FROM node:18-alpine

# 作業ディレクトリを設定
WORKDIR /app

# 依存パッケージ定義ファイルをコピー
COPY package.json package-lock.json ./

# 依存パッケージをインストール
RUN npm install

# アプリケーションコードをコピー
COPY . .

# 開発サーバーを起動
CMD ["npm", "run", "dev"]
