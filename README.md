# GunzScan 🛡️ 📊

**The definitive high-performance analytics platform and explorer for the GUNZ Subnet.**

## 🎯 Overview
GunzScan is not just another blockchain explorer; it's a player-centric command center. While generic explorers focus on hashes and gas, **GunzScan** translates raw on-chain data into meaningful gaming metrics for the *Off The Grid* ecosystem.

Our mission is to bridge the gap between complex blockchain events and the player experience, providing real-time insights into item provenance, market trends, and player economies.

## 🚀 Key Features (Build Games Roadmap)
- **Player-Centric UX:** Search by Player Alias or Wallet to see specialized game inventories.
- **Item Provenance:** Trace the history of a specific NFT (Weapon/Skin) from minting to its current owner, including past battle participation.
- **Market Analytics:** Real-time floor price tracking and volume analysis within the GUNZ Subnet.
- **Developer API:** A high-performance REST/GraphQL API for other builders to fetch processed game data.
- **Deep Metadata Indexing:** Instant filtering by game attributes (Fire rate, Damage, Rarity, etc.).

## 🛠️ Technical Stack (The Senior Approach)
To handle the scale of 20M+ transactions with zero-latency, GunzScan utilizes an event-driven architecture:

- **Indexer:** Node.js/TypeScript service utilizing `viem` for robust RPC polling and event log decoding.
- **Database:** PostgreSQL (via Supabase) with optimized indexing for JSONB metadata.
- **Cache Layer:** Redis for high-frequency market data and global stats.
- **Frontend:** Next.js 14 (App Router) + Tailwind CSS + Tremor for professional-grade analytics dashboards.
- **Infrastructure:** Scalable serverless architecture designed for high availability.

## 🏗️ Architecture Sketch
1. **Extraction Layer:** Polls the GUNZ RPC (`rpc.gunzchain.io`) for `Transfer` and custom game events.
2. **Transformation Layer:** Normalizes raw hex data into human-readable game stats.
3. **Storage Layer:** Relational storage for transactions and document storage for NFT metadata.
4. **Presentation Layer:** A responsive dashboard optimized for both desktop "power-users" and mobile players.

## 📈 Status
- [x] Research & RPC Connection established.
- [ ] Database Schema Design (In Progress).
- [ ] Indexer MVP (Planned).
- [ ] UI/UX Prototype (Planned).

---
*Developed for the **Avalanche Build Games 2026** competition.*
