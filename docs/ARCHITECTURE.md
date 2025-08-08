# Minimal Viable Ledger (MVL) Specification

## Purpose
Implement a single-node ledger capable of:
- Storing blocks containing transactions
- Validating basic transaction structure
- Linking blocks using hashes
- Providing REST API to add & retrieve blocks

## Components
1. **Transaction**
   - `id` (UUID)
   - `timestamp`
   - `payload` (arbitrary JSON)
   - `signature` (string)

2. **Block**
   - `index` (integer)
   - `timestamp`
   - `transactions` (array)
   - `previousHash` (string)
   - `hash` (string)
   - `nonce` (optional)

3. **APIs**
   - `GET /chain` → full blockchain
   - `POST /transaction` → submit transaction
   - `POST /mine` → create block from pending transactions

4. **Persistence**
   - Store chain in LevelDB (later: file/db hybrid)

## Future Enhancements
- Multi-node P2P
- Consensus algorithm
- API versioning
- Angular frontend
