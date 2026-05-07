# Environment Variables Setup

## For Render Deployments

### Python AI Service (mentorshipp-python-api)
```
GROQ_API_KEY=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
```

### Node API Service (mentorshipp-node-api)
```
PORT=5000
MONGO_URI=mongodb://mayank2008mishra08_db_user:avsKRoWtPk1Kz2zd@ac-rr8ff09-shard-00-00.smzhwcq.mongodb.net:27017,ac-rr8ff09-shard-00-01.smzhwcq.mongodb.net:27017,ac-rr8ff09-shard-00-02.smzhwcq.mongodb.net:27017/rediti?ssl=true&replicaSet=atlas-5vedit-shard-0&authSource=admin&appName=Cluster0
AI_SERVICE_URL=https://mentorshipp-python-api.onrender.com
```

### Frontend (Vercel)
After both services are live on Render, add to Vercel:
```
NEXT_PUBLIC_NODE_API_URL=https://mentorshipp-node-api.onrender.com
NEXT_PUBLIC_PYTHON_API_URL=https://mentorshipp-python-api.onrender.com
```

## Local Development (.env files)
Already configured in:
- `server/.env` - For Node server
- `ai_service/.env` - For Python service
- `client/.env.local` - For Next.js frontend
