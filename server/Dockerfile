FROM node:alpine

WORKDIR /app
COPY ./package.json ./
RUN npm install
COPY . .


ENV MONGO_URL=mongodb+srv://ankush:ankush@zomato-master.sh1t9.mongodb.net/zomato?retryWrites=true&w=majority
ENV GOOGLE_CLIENT_ID=982470435364-jhka15s802k9m1n8ja8n3beptacsmjsu.apps.googleusercontent.com
ENV GOOGLE_CLIENT_SECRET=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
ENV AWS_S3_ACCESS_KEY=AKIAX3DBEBNFYY5B6CCN
ENV AWS_S3_SECRET_KEY=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
ENV MAILGUN__DOMAIN=sandboxed1a7739fb7b4222a090b3de2f0c9d38.mailgun.org
ENV MAILGUN__API__KEY=7f8586881bcbf39933eac2bd90574c10-2ac825a1-388d0d9b
ENV RZR_PAY_ID=rzp_test_EvTtQdG4x6tnDp
ENV RZR_PAY_SECRET=t2nuKWYyccx2nDJizV5CehBF
ENV NODE_ENV=production
ENV PORT=4000

RUN npm run build


CMD ["npm", "run", "start"]