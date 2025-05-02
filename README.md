# lld-ride-matching-system
Designing a Ride Matching System (like Uber Pool)

<details><summary><b>Problem Statement</b></summary>

📌 Objective:
Build a simplified ride-matching system that can:
1. Register riders and drivers. 
2. Create ride requests. 
3. Match ride requests with nearby available drivers. 
4. Handle pooling (i.e., allow 2 riders to share a ride if their routes match). 
5. Support basic trip completion and history tracking.

💡 Core Functional Requirements:
1. Register a Rider and Driver 
    - Rider has id, name, and current location (x, y)
    - Driver has id, name, current location (x, y) and isAvailable flag 
2. Request a Ride 
   - Rider requests a ride to a destination (x, y)
   - System should match with: a driver within a certain distance (e.g., 5 units) preferably a driver already going that way (pooling)
3. Pooling Support
   - If another ride is already in progress and has space (say max 2 riders), allow a new rider to join if their origin and destination are reasonably close to the existing trip.
4. End a Ride 
   - When a ride ends, update driver status, remove ride entry
5. List Trip History
   - For each rider, list all past trips with source, destination, matched driver, and ride status
</details>

