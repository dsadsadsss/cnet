FROM node:18-alpine

WORKDIR /app

COPY package.json index.js ./

ENV FILE_PATH=/app \
    SHOW_LOG=false

EXPOSE 7860

CMD ["node", "index.js"]
