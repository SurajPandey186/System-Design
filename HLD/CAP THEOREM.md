
# 📘 CAP Theorem – Complete Notes

## 📌 What is CAP Theorem?

CAP Theorem (also known as Brewer’s Theorem) states that:

> In a Distributed System, you can only guarantee **2 out of the following 3 properties** at the same time:
>
> - **C – Consistency**
> - **A – Availability**
> - **P – Partition Tolerance**

It is impossible to guarantee all three simultaneously.

---

# 🔺 The Three Properties

## 1️⃣ Consistency (C)

**Definition:**
Every read receives the most recent write.

**Meaning:**
- All nodes show the same data at the same time.
- No stale or outdated data.

**Example:**
If you transfer ₹10,000:
- Immediately checking the balance shows updated amount.

---

## 2️⃣ Availability (A)

**Definition:**
Every request receives a response (success or failure).

**Meaning:**
- System never hangs.
- It always responds.
- Data may not always be the latest.

**Example:**
Even during server issues, the system returns some data.

---

## 3️⃣ Partition Tolerance (P)**

**Definition:**
System continues operating despite network failures between nodes.

**Meaning:**
- Servers can’t communicate.
- Network splits into partitions.
- System must still function.

⚠ In distributed systems, network failures are inevitable.

---

# 🚨 The Core Rule

When a **network partition happens**, the system must choose:

- Consistency (C)
OR
- Availability (A)

You cannot guarantee both.

Since Partition Tolerance is mandatory in distributed systems,
you effectively choose between:

- **CP**
- **AP**

---

# 🧩 System Types

## 🔵 CP (Consistency + Partition Tolerance)

- Data is always correct.
- Some requests may fail during partition.

**Used for:**
- Banking systems
- Payment systems
- Financial transactions

---

## 🟢 AP (Availability + Partition Tolerance)

- System always responds.
- Data may be temporarily inconsistent.
- Uses eventual consistency.

**Used for:**
- Social media
- E-commerce carts
- Distributed caches

---

## 🔴 CA (Consistency + Availability)

- Works only if no partition occurs.
- Not realistic for distributed systems.

**Used in:**
- Single-node databases

---

# 📊 Comparison Table

| Type | Consistent Data | Always Responds | Partition Safe | Use Case |
|------|----------------|----------------|----------------|----------|
| CP   | ✅ Yes        | ❌ Sometimes   | ✅ Yes         | Banking |
| AP   | ❌ Eventually | ✅ Yes         | ✅ Yes         | Social Apps |
| CA   | ✅ Yes        | ✅ Yes         | ❌ No          | Single DB |

---

# 🧠 Important Interview Insight

CAP theorem only applies when **network partition occurs**.

If there is no partition:
- System can provide both Consistency and Availability.

But since partitions are unavoidable,
real-world distributed systems are either:

- CP
- AP

---

# 🔥 Real-World Understanding

Imagine two servers:

Server A -----X----- Server B  
(Network link breaks)

Now system must choose:

- Stop serving requests to maintain correctness (CP)
OR
- Keep serving requests but risk inconsistent data (AP)

---

# 📝 Key Takeaways

- CAP applies only to distributed systems.
- Partition tolerance is mandatory.
- You must choose between Consistency and Availability during failure.
- Strong consistency = safer but slower.
- Eventual consistency = faster but temporarily inconsistent.

---

# 📚 Related Concepts (Study Next)

- Strong vs Eventual Consistency
- PACELC Theorem
- Quorum-based Replication
- Leader Election
- Distributed Consensus (Raft / Paxos)

---

# 🚀 Quick Summary

CAP Theorem =  
"In the presence of network failure, you must choose between Consistency and Availability."

You cannot have all three.
