# ProofX
A fully functional blockchain and cryptocurrency system built from scratch. Implements core blockchain concepts including cryptographic hashing, Proof of Work mining, wallet generation, digital signatures, transaction validation, and a distributed node network. Includes a React-based frontend for live blockchain visualization and wallet management.

#### Command To Activate Project

**Activate the virtual environment**
```
blockchain-env/Scripts/activate
```

**Install all packages**
```
pip install -r requirements.txt
```

**Run the tests**

Make sure to activate the virtual environment.

```
python -m pytest backend/tests
```

**Run the application and API**

Make sure to activate the virtual environment.

```
python -m backend.app
```

**Run a peer instance**

Make sure to activate the virtual environment.
Choose a unique PUBNUB_USER_ID per peer.

```
export PEER=True && export PUBNUB_USER_ID=blockchain-peer-1 && python -m backend.app
```

**Run the frontend**

In the frontend directory:
```
npm start
```

**Seed the backend with data**

Make sure to activate the virtual environment.

```
export SEED_DATA=True && python3 -m backend.app
```

** PubNub Configuration**

This application uses PubNub for real-time peer-to-peer communication between blockchain nodes. **You must configure PubNub to run the application.**

**See [PUBNUB_CONFIG.md](PUBNUB_CONFIG.md) for detailed setup instructions.**

1. Get free PubNub keys at [https://www.pubnub.com/](https://www.pubnub.com/)
2. copy `backend/env.example` to `backend/.env` and configure it with your keys.
