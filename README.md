# Dap: A Pragmatic Approach to Decentralized Naming
**Version 9**

## 1. Abstract

The internet’s naming system remains under the centralized control of the Internet Corporation for Assigned Names and Numbers (ICANN), requiring million‑dollar fees and bureaucratic approval processes for new top‑level domains. While other blockchain naming systems have attempted to solve this through pure decentralization, they have failed to produce notable products or use cases after years of operation, trapped by ideological purity that refuses any coordination even when necessary for basic ecosystem development.

Dap represents a pragmatic alternative: decentralized enough to ensure censorship resistance and permissionless innovation, yet coordinated enough to ship products and serve users. We explicitly reject the purity spirals that have paralyzed other projects, choosing instead to measure success by applications built, users served, and utility created.

This paper introduces Dap’s technical architecture, economic model, and our philosophy of pragmatic decentralization that prioritizes shipping over philosophizing. Perfect decentralization without adoption is worthless. Dap chooses adoption.

## 2. Introduction

### 2.1 The Current State of Internet Naming

Since 1998, ICANN has maintained monopolistic control over the internet’s root naming system. Creating a new top‑level domain (TLD) requires:

- A $185,000 non‑refundable application fee
- Years of bureaucratic review processes
- Proof of technical and financial capability
- Compliance with extensive policies and restrictions
- Ongoing contractual obligations and fees

This system has resulted in ~1,500 TLDs existing after decades of internet growth, with control concentrated among a handful of large registry operators. Innovation is stifled, prices remain high, and entire communities and businesses are excluded from owning their namespace.

### 2.2 Why Other Blockchains Failed to Deliver

Previous blockchain naming systems launched with the promise of decentralizing domain names. The technology works; the blockchains run, names can be registered, DNS records can be set. Yet after years:

- **Zero notable products** have been built
- **Zero major websites** use their names
- **Zero services** provide utility to end users
- **The communities have nearly abandoned these projects**

Why? The answer isn’t technical; it’s cultural.

These communities inherited Bitcoin maximalism’s toxic trait: an absolute refusal to coordinate or centralize anything, even temporarily, even when necessary for basic ecosystem development. This manifested as:

**The Purity Trap**: Any suggestion of coordination, funding, or leadership was attacked as “centralization” and rejected, regardless of practical benefits.

**Technical Superiority Complex**: Communities became satisfied with having built “the best decentralized naming system” technically, while ignoring that nobody uses it.

**Governance Paralysis**: Decision‑making processes optimized for “decentralization theater” over progress. Months spent debating, zero time shipping.

**User Hostility**: Expecting end users to understand blockchain mechanics, run full nodes, and compile software from source. Then wondering why adoption never came.

**The Field of Dreams Fallacy**: “Build the infrastructure and they will come.” No marketing. No business development. No user onboarding. No ecosystem cultivation.

Dap explicitly rejects this failed approach. We prioritize pragmatism, product development, and user adoption over ideological purity.

### 2.3 The Dap Philosophy

**Products Over Protocol**: We judge ourselves by applications built and users served, not by technical papers published or governance proposals debated.

**Pragmatic Decentralization**: We use centralization as a tool when it accelerates development, with clear sunset provisions to prevent permanent capture.

**User‑First Design**: If your grandmother can’t use it, we haven’t built it right. Complexity belongs in the backend, not the user interface.

**Aggressive Business Development**: We don’t wait for organic adoption. We actively pursue partnerships, integrations, and users.

**Rapid Iteration**: We ship weekly, not yearly. Better to launch and fix than to debate and delay.

## 3. Market Opportunity

### 3.1 The Domain Name Industry

The domain industry generates over $10 billion annually, with:

- 350+ million registered domains
- Average prices of $10‑50 per year
- Premium domains selling for millions
- Entire secondary market of brokers and investors

Yet innovation has stagnated:

- Same TLD application process since 2012
- Same registrar/registry split model
- Same centralized control structure
- Same barriers to entry

### 3.2 Dap’s Opportunity

Dap targets three distinct markets:

**TLD Ownership**: Instead of paying ICANN $185,000+ and waiting years, own a TLD on Dap immediately through transparent auctions.

**Brand Protection**: Companies can own their .brand TLD forever, controlling their entire namespace without annual ICANN fees.

**Developer Innovation**: Build applications impossible under ICANN’s restrictions—token‑gated domains, NFT integration, automated markets.

### 3.3 Go‑to‑Market Strategy

Unlike projects that wait for users to discover them, Dap actively creates adoption:

**Phase 1: Resolution & Builders (Months 0‑6)**

- Browser extensions for Chrome, Firefox, Safari at launch
- Public DoH/DoT resolver (`dns.dap.sh`) at launch
- Developer grants program ($10M allocated)
- Weekly hackathons and demo days
- Technical documentation and SDKs
- Direct outreach to Web3 projects

**Phase 2: Browser & Businesses (Months 6‑12)**

- Aries browser ships (Chromium engine)
- Native browser integration negotiations
- Enterprise sales team targeting Fortune 500
- White‑glove onboarding for major brands
- Partnership with existing registrars
- Integration with popular platforms

**Phase 3: Mass Adoption (Months 12+)**

- Mobile apps for iOS/Android with built-in resolution
- Marketing campaigns targeting specific communities
- Influencer partnerships and sponsorships
- Consumer education initiatives

**Pragmatic Governance**: For the first two years, a small team makes decisions quickly. No months‑long governance debates about minor technical details. No committee paralysis. Decisions in days, not months.

We choose building over debating, shipping over philosophizing, and users over ideology.

## 4. Technical Architecture

### 4.1 Blockchain Layer

Dap builds on proven foundations while fixing the limitations of previous systems. We use a UTXO‑based blockchain with enhanced covenants designed for domain name operations.

**Core Design Principles**:

- UTXO model for simplicity and scalability
- Proof‑of‑work for objective security
- Covenant system for native naming operations
- Open participation without permission

**Key Improvements**:

- Simplified covenant types focused on realistic use cases
- Enhanced scripting for complex TLD management
- Optimized block structure for DNS data
- Production‑ready immediately, not “eventually”

We resist the temptation to over‑engineer. Every technical decision is evaluated against realistic use cases, not theoretical possibilities.

### 4.2 Consensus: Practical Innovation

Dap implements a revolutionary consensus mechanism combining three proven technologies:

**Verifiable Delay Functions (VDF)**: Replace pure computational work with time‑based proofs, reducing energy consumption by 95% while maintaining security. Miners prove elapsed time, not wasted computation.

**Verifiable Random Functions (VRF)**: Provide provably fair randomness for block producer selection and auction resolution. No more mining pool centralization or auction manipulation.

**Blake3 Proof‑of‑Work**: The fastest cryptographic hash function available, providing efficient verification.

This “Trinity” design delivers:

- 95% energy reduction versus traditional PoW
- Predictable 2‑minute block times
- Fair mining distribution without pools
- Sustainable security model

But we emphasize: **Technical superiority means nothing without adoption**. We judge our consensus by whether it enables products, not whether it wins academic awards.

### 4.3 Resolution: The Existential Priority

A naming system nobody can resolve is a naming system nobody uses. Resolution isn’t a feature—it’s the entire product. Without it, we’re selling vanity database entries.

**Day One Requirements** (Ship with mainnet or don’t launch):

- Browser extensions for Chrome, Firefox, Safari
- Public DoH resolver at `dns.dap.sh`
- Public DoT resolver for system-level integration
- Mobile DNS configuration profiles
- CLI tools for developers

**Year One Goals**:

- Aries browser with native resolution (Chromium first, WebKit and Servo to follow)
- Integration discussions with major browsers
- ISP partnership pilots
- Enterprise resolver deployments

**Technical Specifications**:

- Full DNS protocol support (RFC compliant)
- DNSSEC implementation
- Response time under 50ms
- 99.9% uptime SLA
- IPv4 and IPv6 support

**Advanced Features**:

- SSH fingerprints (SSHFP)
- TLS certificate pinning (TLSA)
- Email authentication (DKIM/SPF/DMARC)
- Custom record types for Web3

**Measurable Success**:

- Daily query volume tracking
- Resolution success rate
- User adoption metrics
- Geographic distribution

**Users shouldn’t need to understand blockchain to use blockchain domains.** They type a URL, it resolves. Everything else is implementation detail.

## 5. Ecosystem Development Strategy

### 5.1 The Anti‑Maximalist Approach

Where other projects relied on spontaneous emergence, Dap actively cultivates its ecosystem:

**Centralized Kickstart**: The Dap Foundation initially coordinates development, funds builders, and drives adoption. This is temporary centralization for permanent decentralization. We’ll sunset the foundation’s special powers after achieving product‑market fit.

**Developer Grants**: $10 million allocated for builders who ship products. Not researchers who write papers, not theorists who debate governance—builders who ship code users can use.

**Marketing Budget**: Yes, we market. We advertise. We sponsor conferences. We create content. We do business development. Because products without users are expensive hobbies.

**Business Development**: We actively pursue partnerships with registries, browsers, and applications. We don’t wait for organic adoption—we create it.

### 5.2 Product‑First Roadmap

Our success metrics are products and users, not protocol features:

**Testnet Goals**:

- 10+ working applications before mainnet
- 1,000+ active developers building
- 10,000+ daily active testnet users
- Businesses testing use cases

**Product Showcases**:

- Weekly demo days for new applications
- Monthly builder spotlights
- Quarterly ecosystem reports
- Annual developer conference

**User Focus**:

- Onboarding guides for non‑technical users
- One‑click setup tools
- Customer support
- User feedback integration

Every protocol decision is downstream from “What helps users?”

### 5.3 Builder Incentives

We explicitly favor builders over speculators:

**Testnet Rewards**: Developers who build during testnet receive GRP token grants at mainnet launch. The more you build, the more you earn.

**Mainnet Allocation**: 10% of token supply reserved for proven builders, distributed based on ecosystem contribution, not token holdings.

**Revenue Sharing**: TLD auction revenues partially distributed to application developers driving adoption. Build the ecosystem, share the rewards.

**Anti‑Speculation Measures**:

- TLD owners must demonstrate usage within 1 year or face reclaim
- Multiple TLD ownership requires proven utilization of existing TLDs
- Squatting penalties fund builder grants

We want builders, not holders. Users, not speculators. Products, not promises.

## 6. TLD Auction System

### 6.1 Designed for Use, Not Speculation

Dap’s auction system prioritizes utilization:

**Vickrey Auction Format**: Blind second‑price auctions ensure fair price discovery. Bidders submit sealed bids; the winner pays the second‑highest bid amount. This mechanism encourages honest bidding; your dominant strategy is to bid your true valuation, while preventing bid sniping and last‑minute manipulation.

**Progressive Minimums**:

- Single‑letter TLDs: 100K GRP minimum
- Two‑letter TLDs: 10K GRP minimum
- Three‑letter TLDs: 1K GRP minimum
- Generic TLDs: 100 GRP minimum

**Build Requirements**: TLD winners must:

- Set nameservers within 30 days
- Demonstrate registration system within 90 days
- Show active usage within 1 year
- Or face automatic reclaim and re‑auction

**Builder Advantages**:

- Proven developers get 20% auction discount
- Ecosystem contributors get priority access
- Multiple TLD bids require utilization proof

### 6.2 Registry Flexibility

TLD owners have complete control over their namespace:

**Business Models**:

- Traditional: Charge registration fees
- Free: Build ecosystem through free domains
- Token‑Gated: Require NFT/token ownership
- Verified: KYC/identity requirements
- Custom: Any model you can imagine

**Technical Freedom**:

- Choose any registry software
- Set any DNS records
- Implement any policies
- Run any infrastructure

**The Crucial Insight**: “Own the whole `.com`, not just a domain.” Instead of registering `mycompany.com`, own `.mycompany` and control unlimited domains beneath it.

### 6.3 Anti‑Squatting Mechanisms

TLD squatting is prevented through economic incentives:

**Usage Requirements**:

- Year 1: Must have 100+ domains registered
- Year 2: Must have 1000+ domains registered
- Or pay 10x renewal fee for unused TLDs

**Renewal Scaling**:

- Active TLD: 1000 GRP/year
- Low‑use TLD (<100 domains): 10,000 GRP/year
- Unused TLD (0 domains): 100,000 GRP/year
- Automatic reclaim after 2 years unused

**Bulk Penalties**:

- 1 TLD: Normal price
- 10 TLDs: 2x price each
- 100 TLDs: 5x price each
- Message: You better use them!

### 6.4 Personal TLDs

Standard TLDs require SLD registrations to prevent squatting, but this conflicts with a legitimate use case: personal namespaces. Someone wanting `.lanhikari` for their own identity shouldn’t need (nor want) to sell domains to strangers.

Personal TLDs solve this through economic design rather than honor systems.

**Registration Choice**

At TLD claim, the wallet selects one of two classes:

| Class    | Renewal Fee  | SLD Requirement           | Transfer Rules      |
|----------|--------------|---------------------------|---------------------|
| Standard | Base rate    | 100+ Year 1, 1000+ Year 2 | Freely transferable |
| Personal | 3× base rate | None                      | Graduated unlock    |

The choice is recorded on‑chain at registration. The 3× fee multiplier makes portfolio‑building uneconomical while remaining affordable for genuine personal use.

**Graduated Transfer Unlock**

Personal TLDs have transfer restrictions that decay over time:

| Ownership Duration | Transfer Allowed? | Burn Penalty             |
|--------------------|-------------------|--------------------------|
| Year 0–1           | No                | Blocked                  |
| Year 1–2           | Yes               | 75% of sale price burned |
| Year 2–3           | Yes               | 50% of sale price burned |
| Year 3+            | Yes               | None                     |

**Deflationary burns**: All penalty burns permanently remove GRP from circulation. No treasury allocation—pure deflation. This ensures no constituency benefits from rule‑breaking, making the penalty a pure disincentive.

By year 3, the owner has paid enough premium renewals (3× annually) that speculation math doesn’t work regardless of transfer freedom.

**Personal → Standard Conversion**

Circumstances change. A personal TLD can convert to standard class at any time, with the following conditions:

1. SLD requirement activates immediately (clock starts, usage thresholds apply)
2. Transfer lock resets to year 0 of the standard transfer schedule
3. Renewal fee drops to base rate on the next renewal cycle
4. Conversion is irreversible

This prevents gaming where someone parks as personal then flips to standard right before a sale. The reverse conversion (standard → personal) is not permitted.

**On-Chain Data**

```
TLD {
  class: "personal" | "standard";
  last_renewed: timestamp;
  name: string;
  personal_since: timestamp | null;
  registered_at: timestamp;
}
```

The `personal_since` field tracks when the TLD entered personal class, enabling accurate graduated unlock calculations regardless of original registration date.

**Design Rationale**

This approach succeeds where cap‑based exemptions (e.g., “4‑10 personal TLDs per wallet”) would fail:

- **No Sybil vulnerability**: Creating multiple wallets doesn’t help—each TLD costs 3× to maintain
- **Self‑enforcing**: No subjective judgment calls or governance overhead
- **Clear social contract**: “Personal TLDs are yours, not investment vehicles”—the restrictions become a feature

## 7. Governance: Efficient, Not Perfect

### 7.1 Benevolent Dictatorship Phase

For the first two years, the Dap Foundation makes decisions quickly:

- Protocol upgrades decided in days, not months
- Resource allocation without committees
- Partnership negotiations without votes
- Emergency responses without delays

This is explicitly temporary. We need to achieve product‑market fit before decentralizing governance. Other projects proved that premature decentralization equals permanent paralysis.

### 7.2 Practical Decentralization

After two years, we transition to community governance with pragmatic constraints:

**Bounded Decisions**: Governance for major changes (protocol upgrades, economic parameters). Daily operations remain centralized for efficiency.

**Time Limits**: All proposals have 30‑day maximum discussion periods. Decisions happen, even if imperfect.

**Implementation Focus**: Proposals must include implementation plans, not merely ideas. “Who will build this?” comes before “Should we build this?”

**Default to Action**: Without clear consensus against, we proceed. Inaction is not an option.

### 7.3 Sunset Provisions

All special powers expire automatically:

| Component           | Initial Control | Transition      | Final State                    |
|---------------------|-----------------|-----------------|--------------------------------|
| Development Fund    | Foundation      | -20% yearly     | Community DAO by Year 5        |
| Technical Decisions | Core Team       | Gradual opening | Full community by Year 3       |
| Marketing           | Dedicated Team  | Ongoing         | Professional team (DAO funded) |
| Partnerships        | Business Dev    | Ongoing         | Professional team (DAO funded) |

## 8. Token Economics

### 8.1 GRP Token Distribution

Total Supply: **420,000,000 GRP**

The base denomination is the **grippie** (plural: grippies). 1 GRP = 100,000,000 grippies, analogous to Bitcoin’s satoshi. All consensus math operates on grippies as integer values; floating‑point arithmetic is never used.

**Distribution**:

- Mining Rewards: 70% (294M GRP)
- Developer Fund: 10% (42M GRP)
- Ecosystem Grants: 7.5% (31.5M GRP)
- Treasury: 7.5% (31.5M GRP)
- Advisors: 2.5% (10.5M GRP)
- Marketing: 2.5% (10.5M GRP)

**Why 70% to Miners**: Unlike other projects that waste tokens on unclaimed airdrops or insider allocations, Dap puts the overwhelming majority in the hands of those securing the network. Miners are the backbone of Dap.

### 8.2 Deflationary Mechanics

All TLD auction proceeds and penalty burns are permanently removed from circulation:

**Burn Sources**:

- TLD auction winning bids
- Personal TLD early transfer penalties (graduated 75%/50%)
- Future protocol‑level penalties

**Burn Projections**:

- Year 1: 1‑2M GRP burned
- Year 5: 10‑15M GRP burned cumulative
- Year 10: 25‑35M GRP burned cumulative
- Long‑term: 5‑10% of supply permanently removed

**Economic Security**: As supply decreases through burning while demand increases through adoption, GRP becomes increasingly valuable, ensuring long‑term mining incentives even as block rewards decrease.

**Why True Burns**: Penalty burns go to a provably unspendable address rather than a treasury. This eliminates perverse incentives—no constituency profits from rule‑breaking. “Break the rules, value disappears” is simpler to explain and harder to politicize than redistribution schemes.

### 8.3 No Pre-mine Games

Unlike other projects with complex token swaps or conversion mechanisms:

- **Pure GRP from the start**: No confusion, no conversion rates
- **No insider advantages**: Everyone starts equal
- **No wasted allocations**: Every GRP has a purpose
- **Clear value proposition**: “420M GRP. 70% to miners. 30% to builders.”

## 9. A True Alternative Root

### 9.1 The Competition ICANN Never Had

ICANN has operated without meaningful competition for decades. No pressure to innovate. No incentive to lower prices. No reason to improve. Dap changes that.

**We are not an extension of the existing internet. We are an alternative.**

**No Reserved Namespaces**: Every TLD is available at genesis. `.com`, `.google`, `.amazon`—all of it. If Verisign wants `.com` on Dap, they can bid in the auction like everyone else. We don’t reserve their seat at our table.

**No Special Treatment**: Legacy operators have no automatic claims, no DNSSEC proof shortcuts, no priority access. Dap is a level playing field. Your ICANN credentials mean nothing here—only your willingness to build and your GRP to bid.

**No Apologies**: We’re not “complementing” ICANN or “coexisting peacefully.” We’re demonstrating what a root namespace looks like when it’s run for users instead of bureaucrats. If that’s threatening, good. Competition should be.

### 9.2 The Bitcoin Precedent

Bitcoin didn’t ask permission from central banks. It didn’t say “we’ll avoid fiat currency denominations to prevent confusion.” It built an alternative monetary system and let people choose.

Dap follows the same logic. We’re not asking ICANN’s permission. We’re not worried about “name conflicts” with their system. We’re building something better and letting the market decide.

**Your resolver, your namespace, your choice.**

### 9.3 Resolution Is the Battlefield

The only question that matters: can users reach Dap domains?

If yes, we win. ICANN becomes one option among many—the legacy option, the expensive option, the slow option.

If no, we’re irrelevant. The best protocol in the world means nothing if nobody can use it.

This is why resolution ships Day One. Not Year 3. Not “eventually.” Day One.

**Resolution Strategy**:

| Approach                                     | Timeline         | Reach                           |
|----------------------------------------------|------------------|---------------------------------|
| Browser extensions (Chrome, Firefox, Safari) | Launch           | Early adopters, developers      |
| Public DoH/DoT resolver (`dns.dap.sh`)       | Launch           | Anyone who changes DNS settings |
| Mobile configuration profiles                | Launch           | iOS/Android users               |
| Aries browser (Chromium)                     | Year 1           | Full native experience          |
| Aries browser (WebKit, Servo)                | Year 1-2         | Engine diversity                |
| ISP partnerships                             | Year 1-2         | Mainstream users                |
| Native browser integration                   | Ongoing          | Mass adoption (the real goal)   |

### 9.4 What Happens to “Conflicts”?

Someone owns `.google` on Dap. Google Inc. is unhappy. What happens?

**Nothing special.** Google can:

1. Bid on `.google` in Dap’s auction (they probably should)
2. Ignore Dap entirely (their choice)
3. Sue someone (good luck—we’re decentralized)

What Google cannot do: demand we reserve their name, expect special treatment, or dictate our namespace policy.

The Dap owner of `.google` has exactly the same rights as every other TLD owner. They must meet usage requirements or face reclaim. If they squat, they pay escalating fees. If they build, they thrive.

**Trademarks are an ICANN concern.** In Dap’s namespace, you own what you win. Build something or lose it.

## 10. The Anti‑Maximalist Manifesto

### 10.1 What We’re NOT

- **Not asking ICANN’s permission**: We compete, we don’t petition
- **Not purely decentralized**: We coordinate when necessary
- **Not waiting for perfection**: We ship when good enough
- **Not hostile to business**: We embrace commercial success
- **Not ideologically driven**: We’re results driven
- **Not building for cypherpunks**: We’re building for everyone

### 10.2 What We ARE

- **Building products**: Code running in production
- **Shipping working code**: Weekly releases, not yearly promises
- **Growing an ecosystem**: Active developer relations and support
- **Creating utility**: Solving genuine problems for genuine users
- **Embracing pragmatism**: The best solution that ships
- **Measuring success**: By usage, not ideology

### 10.3 Our Metrics

**What We Track**:

- GitHub commits per week
- New applications launched
- Active users (daily/monthly)
- DNS queries served
- Revenue generated
- Developer satisfaction

**What We Don’t Track**:

- Governance participation
- Decentralization scores
- Token price speculation
- Ideological purity
- Community sentiment
- Social media followers

Build. Ship. Iterate. Everything else is noise.

## 11. Why Dap Will Succeed Where Others Failed

### 11.1 Leadership Exists

Unlike other projects’ headless approach, Dap has clear leadership:

**Technical Direction**: Core team makes architectural decisions quickly and decisively. No endless bike-shedding over minor details.

**Ecosystem Coordination**: Dedicated team manages developer relations, partnerships, and user growth. Not left to “emerge organically.”

**Resource Allocation**: Foundation distributes grants based on results, not politics. Ship code, get funded.

**Accountability**: Leaders have genuine names, genuine reputations, and genuine skin in the game. No hiding behind anonymous accounts.

### 11.2 Sustainable Economics

**For Miners**: 70% of supply ensures profitable mining even at low token prices. No dependency on unsustainable subsidies.

**For Developers**: Direct grants, revenue sharing, and clear monetization paths. Build on Dap, make money.

**For Users**: Utility from the start. Use domains for websites, email, identity. Not only speculation.

**For TLD Owners**: Run a genuine business selling domains. Not merely holding and hoping.

### 11.3 Pragmatic Timeline

**Year 0 (Testnet)**: Build, test, iterate. Browser extensions and resolver ready. Launch when ready, not when scheduled.

**Year 1**: Browser extensions live, Aries browser shipped, 10+ production applications, 100+ active developers, 10K+ daily users.

**Year 2**: Native browser integration negotiations, enterprise adoption, 100K+ daily users.

**Year 3**: Mainstream awareness, 1M+ daily users, profitable ecosystem.

**Year 5**: Serving 1B+ DNS queries daily. Undeniable product‑market fit.

## 12. Conclusion

Dap represents a fundamental shift in how blockchain projects approach development and adoption. We reject the failed maximalist approach that prioritizes ideological purity over user value. We embrace pragmatic trade‑offs that enable us to ship products and serve users.

The domain name system is too important to leave in the hands of:

- ICANN’s bureaucracy and gatekeeping
- Blockchain projects that refuse to ship
- Ideological purists who hate users
- Speculators who build nothing

Dap will succeed because we:

- Ship code weekly, not yearly
- Pursue users aggressively, not passively
- Build products people want, not protocols nobody uses
- Measure success by adoption, not ideology
- Compete directly instead of asking permission

The internet deserves a naming system that is both decentralized AND useful. Previous projects proved you can build one or the other. Dap will prove you can build both.

ICANN has had no competition for three decades. That ends now.

Join us in building the future of internet naming. Not through endless debates and governance theater, but through shipping code and serving users.

**Dap: The competition ICANN never had.**

---

## Appendices

### Appendix A: Technical Specifications

#### A.1 Blockchain Parameters

| Parameter              | Value                                 |
|------------------------|---------------------------------------|
| Block time             | 2 minutes (120 seconds)               |
| Block size             | 4 MB maximum                          |
| Consensus              | VDF + VRF + Blake3 PoW                |
| Token                  | GRP                                   |
| Base denomination      | grippies                              |
| Conversion             | 1 GRP = 100,000,000 grippies          |
| Total supply           | 420,000,000 GRP (4.2 × 10¹⁶ grippies) |
| Halving interval       | 1,050,000 blocks (~4 years)           |
| Initial block reward   | 140 GRP                               |
| Minimum TX fee         | 0.01 GRP (1,000,000 grippies)         |
| Dust threshold         | 546 grippies                          |
| Difficulty adjustment  | Every 720 blocks (~24 hours)          |
| Adjustment range       | 0.25× – 4× per period                 |

#### A.2 Consensus: The Trinity

Dap’s consensus combines three cryptographic mechanisms that must all pass for a block to be valid.

##### Verifiable Delay Function (VDF)

| Parameter              | Value                                                          |
|------------------------|----------------------------------------------------------------|
| Scheme                 | Wesolowski (2019)                                              |
| Modulus                | RSA‑2048 challenge number (617 digits, no known factorization) |
| Security parameter     | 128 bits                                                       |
| Duration               | 10 seconds (mainnet), 0.1 seconds (regtest)                    |
| Iteration rate         | ~100,000 iterations/second                                     |
| Production iterations  | ~1,000,000 per block                                           |
| Proof size             | 512 bytes (256‑byte output + 256‑byte proof)                   |

The VDF challenge is the previous block’s hash (32 zero bytes for genesis). Proof generation computes g^(2^t) mod N via t sequential squarings—inherently serial, impossible to parallelize. Verification uses the Wesolowski equation: y = π^l · g^r mod N, where l is a 128‑bit challenge prime derived via Fiat‑Shamir and r = 2^t mod l. Verification runs in O(log t) time, making it orders of magnitude faster than generation.

**Purpose**: Enforces temporal ordering between blocks. No amount of computational resources can produce a valid VDF proof faster than the required delay, preventing timestamp manipulation and ensuring minimum spacing between blocks.

##### Verifiable Random Function (VRF)

| Parameter        | Value                                            |
|------------------|--------------------------------------------------|
| Scheme           | ECVRF‑SECP256K1‑SHA256‑TAI (RFC 9381)            |
| Curve            | secp256k1                                        |
| Suite byte       | 0x01                                             |
| Hash‑to‑curve    | Try‑and‑increment (up to 256 attempts)           |
| Proof size       | 97 bytes (33‑byte gamma + 32‑byte c + 32‑byte s) |
| Output size      | 32 bytes                                         |
| Nonce derivation | Deterministic (RFC 6979‑style)                   |

The VRF input is the previous block’s hash. The miner computes a proof using their private key; the resulting 32‑byte output is compared against a VRF difficulty target. If output ≤ target, the miner is eligible to produce the next block. Ineligible miners skip immediately—no energy wasted on VDF or PoW computation.

Proof‑to‑hash follows RFC 9381 §5.2: output = SHA‑256(suite ‖ 0x03 ‖ gamma), ensuring the random output is uniformly distributed and cannot be biased.

**Purpose**: Provides provably fair, unpredictable block producer selection. Eligibility is tied to a specific private key and cannot be delegated, preventing mining pool centralization.

##### Blake3 Proof‑of‑Work

| Parameter     | Value                                        |
|---------------|----------------------------------------------|
| Hash function | Blake3                                       |
| Input         | Serialized header (786 bytes) ‖ 8‑byte nonce |
| Target        | 32‑byte big‑endian threshold                 |
| Verification  | Single hash comparison                       |

The miner searches for a nonce such that Blake3(header ‖ nonce) ≤ blake3Target. Blake3 is the fastest general‑purpose cryptographic hash function available, providing efficient verification with a single hash operation and low ASIC incentive due to lower PoW difficulty requirements enabled by VRF pre-filtering.

**Purpose**: Provides Byzantine fault tolerance and Sybil resistance. The PoW difficulty is adjusted independently from VRF difficulty—both retarget every 720 blocks but track separate targets.

##### How the Trinity Interlocks

Block production proceeds in three sequential stages:

1. **VRF eligibility check** (~15 ms): Compute VRF proof and check output ≤ vrfTarget. If ineligible, stop immediately.
2. **VDF proof generation** (~10 seconds): Compute Wesolowski VDF over previous block’s hash. Enforces minimum wall‑clock delay.
3. **Blake3 PoW mining** (variable): Search for valid nonce against blake3Target. Duration depends on difficulty and hashrate.

Block validation reverses the cost profile—cheapest rejections first:

1. **VDF verification** (~10 ms): Verify Wesolowski equation.
2. **VRF verification** (~1 ms): Recompute output from miner’s public key, verify eligibility.
3. **Blake3 PoW verification** (~1 μs): Recompute single hash, compare against target.

All three must pass. A block failing any check is rejected.

**Security guarantees**:

- VDF prevents fast‑forwarding: no parallelism produces a valid proof faster than the required delay
- VRF prevents centralization: eligibility is per‑key and non‑transferable
- Blake3 PoW prevents costless block production: real computational work is required

#### A.3 Block Header

The block header is ~858 bytes (compared to Bitcoin’s 80 bytes), reflecting the additional proof data required by Trinity consensus.

| Field          | Size      | Encoding          | Description                        |
|----------------|-----------|-------------------|------------------------------------|
| Version        | 4 bytes   | uint32 LE         | Protocol version                   |
| PrevBlock      | 32 bytes  | raw               | Hash of previous block             |
| MerkleRoot     | 32 bytes  | raw               | Blake3 merkle root of transactions |
| NamesRoot      | 32 bytes  | raw               | Name state Merkle root (see below) |
| Timestamp      | 8 bytes   | uint64 LE         | Unix timestamp (seconds)           |
| VDF Output     | 256 bytes | raw               | Wesolowski VDF computed value      |
| VDF Proof      | 256 bytes | raw (zero‑padded) | Wesolowski proof π                 |
| VDF Iterations | 4 bytes   | uint32 LE         | Number of sequential iterations    |
| VRF Gamma      | 33 bytes  | compressed point  | VRF proof point                    |
| VRF C          | 32 bytes  | raw               | VRF challenge scalar               |
| VRF S          | 32 bytes  | raw               | VRF response scalar                |
| VRF Output     | 32 bytes  | raw               | 32‑byte pseudorandom output        |
| Miner Pubkey   | 33 bytes  | compressed point  | Miner’s secp256k1 public key       |
| Blake3 Nonce   | 8 bytes   | uint64 LE         | PoW nonce                          |
| VRF Target     | 32 bytes  | raw               | VRF difficulty target              |
| Blake3 Target  | 32 bytes  | raw               | Blake3 difficulty target           |

**Block hash**: Blake3(Version through Miner Pubkey ‖ Blake3 Nonce). The hash covers 786 bytes of header data plus the 8‑byte nonce. VRF Target and Blake3 Target are excluded from the hash input—they are consensus‑derived values, not miner‑chosen.

**Merkle tree**: Blake3‑based binary tree over transaction hashes (not double‑SHA256).

**NamesRoot**: A Blake3 Merkle tree over all actively owned TLDs. Only names in ownership states (REGISTER, UPDATE, RENEW, TRANSFER) are included; names still in auction (OPEN, BID, REVEAL) are excluded. Each leaf is the Blake3 hash of a canonical string encoding the name’s hash, covenant state, registration height, owner, expiration block, TLD class, and personal‑since height. Leaves are sorted deterministically by name hash before tree construction, ensuring all nodes compute an identical root. Validators recompute the NamesRoot after processing a block’s covenants and reject any block whose header commitment does not match.

#### A.4 Covenant Types

Dap uses 9 covenant types (byte values 0–8). Unlike some UTXO naming systems, Dap does not implement CLAIM, REDEEM, or REVOKE covenants; their functions are handled by REGISTER and PENALIZE instead.

| Value | Type       | Description                                 |
|-------|------------|---------------------------------------------|
| 0     | `NONE`     | Standard transaction (no covenant)          |
| 1     | `OPEN`     | Initiate a TLD auction                      |
| 2     | `BID`      | Place a sealed bid                          |
| 3     | `REVEAL`   | Reveal a previously sealed bid              |
| 4     | `REGISTER` | Claim TLD ownership (auction winner)        |
| 5     | `UPDATE`   | Update TLD DNS records                      |
| 6     | `RENEW`    | Renew TLD registration                      |
| 7     | `TRANSFER` | Transfer TLD to a new owner                 |
| 8     | `PENALIZE` | Anti‑squatting enforcement (consensus‑only) |

PENALIZE cannot be submitted in user transactions. The consensus layer generates penalize actions automatically at every enforcement interval (2,016 blocks, ~2.8 days).

**State machine**:

```
NONE ——→ OPEN
OPEN ——→ BID
BID  ——→ BID (multiple bids per auction)
BID  ——→ REVEAL
REVEAL → REGISTER
REGISTER ——→ UPDATE / RENEW / TRANSFER
UPDATE   ——→ UPDATE / RENEW / TRANSFER
RENEW    ——→ UPDATE / RENEW / TRANSFER
TRANSFER ——→ UPDATE / RENEW / TRANSFER
PENALIZE ——→ OPEN (triggers re‑auction)
```

**Auction timing (mainnet)**:

| Phase                 | Duration  | Block count | Description                    |
|-----------------------|-----------|-------------|--------------------------------|
| OPEN → BID end        | ~5 days   | 3,600       | Sealed bids accepted           |
| BID end → REVEAL end  | ~1 day    | 720         | Bidders reveal sealed bids     |
| REVEAL end → REGISTER | Immediate | —           | Winner may claim at any time   |
| Expiration            | ~6 months | 131,400     | TLD expires if not renewed     |
| Renewal window        | ~1 month  | 21,900      | Grace period before expiration |

Full lifecycle: OPEN at block N → bids accepted until N+3,600 → reveals accepted until N+4,320 → winner registers after N+4,320 → registration expires at registration block + 131,400.

**Minimum bids by TLD length**:

| TLD length    | Minimum bid | In grippies        |
|---------------|-------------|--------------------|
| 1 character   | 100,000 GRP | 10,000,000,000,000 |
| 2 characters  | 10,000 GRP  | 1,000,000,000,000  |
| 3 characters  | 1,000 GRP   | 100,000,000,000    |
| 4+ characters | 100 GRP     | 10,000,000,000     |

#### A.5 Cryptographic Primitives

All cryptographic operations use audited, constant‑time implementations from the `@noble` library family.

**Hash functions**:

| Algorithm   | Usage                                                                                                           |
|-------------|-----------------------------------------------------------------------------------------------------------------|
| Blake3      | Block hashing, PoW, merkle trees, sighash, name hashing, blind hash computation                                 |
| SHA‑256     | VDF internals (hash‑to‑group, hash‑to‑prime, Fiat‑Shamir), VRF (hash‑to‑curve, challenge, proof‑to‑hash, nonce) |
| RIPEMD‑160  | hash160 = SHA‑256 then RIPEMD‑160, used for address derivation                                                  |

**Signature scheme**: ECDSA over secp256k1 exclusively. Recoverable signatures with DER encoding. No Schnorr or ed25519 in consensus.

**Sighash types**:

| Value | Type                |
|-------|---------------------|
| 0x01  | `SIGHASH_ALL`       |
| 0x02  | `SIGHASH_NONE`      |
| 0x03  | `SIGHASH_SINGLE`    |
| 0x80  | `ANYONECANPAY` flag |

Sighash digests are computed with Blake3, not double‑SHA256.

**Key derivation and encryption**:

| Primitive  | Usage                                    |
|------------|------------------------------------------|
| AES‑GCM    | Symmetric encryption                     |
| PBKDF2     | Password‑based key derivation            |
| HKDF       | Key expansion                            |
| HMAC       | Message authentication (SHA‑256/SHA‑512) |
| scrypt     | Wallet file encryption                   |

**Address encoding**: Bech32 (BIP‑173 compatible) with human‑readable prefix, witness version, and data payload.

#### A.6 Network Configuration

| Network | P2P Port | RPC Port | Wallet Port | Magic Bytes  |
|---------|----------|----------|-------------|--------------|
| Mainnet | 12038    | 12039    | 14038       | `0xd4f00d42` |
| Testnet | 13038    | 13039    | 15038       | `0xd4f00d43` |
| Regtest | 14038    | 14039    | 16038       | `0xd4f00d44` |

#### A.7 P2P Protocol

**Message format**: Every P2P message has a 9‑byte header followed by a variable‑length payload.

| Field          | Size    | Description                    |
|----------------|---------|--------------------------------|
| Magic          | 4 bytes | Network identifier (LE uint32) |
| Command        | 1 byte  | Packet type enum               |
| Payload length | 4 bytes | Payload size (LE uint32)       |

Maximum message size is 8 MB. The magic bytes in every message header must match the network; mismatches cause immediate disconnection.

**Connection limits**: 8 outbound and 8 inbound peers by default, up to 50 total. Production configurations scale inbound limits higher.

**Handshake**: On connect the initiating peer sends a VERSION message (version, services, timestamp, addresses, random nonce, user agent, chain height, relay preference). The remote responds with its own VERSION followed by VERACK. Self‑connections are detected via nonce comparison. Peers below protocol version 70000 are rejected.

**Transport encryption**: Optional TLS 1.3 at the TCP layer. Production mainnet configuration requires it (cipher suites: TLS_AES_256_GCM_SHA384, TLS_CHACHA20_POLY1305_SHA256, TLS_AES_128_GCM_SHA256). Testnet and regtest allow plaintext.

**Peer scoring**: Each misbehavior adds points toward a ban threshold of 100. Reaching the threshold results in a 24‑hour ban. Examples: invalid block announcement (+50), excessive inventory items (+25), transaction rate‑limit violation (+20), unknown message type (+10), rejected transaction (+5). A separate 0‑1 quality score (starting at 0.5) tracks long‑term peer reliability; peers dropping below 0.1 are banned.

**DNS Integration**:

- Full RFC compliance
- DNSSEC support
- < 50ms resolution target
- 99.9% uptime SLA
- IPv6 and IPv4 support

### Appendix B: Pragmatic Trade‑offs

**What Centralization We Accept**:

| Component           | Centralization        | Duration | Justification       |
|---------------------|-----------------------|----------|---------------------|
| Development Fund    | Foundation controlled | 5 years  | Bootstrap ecosystem |
| Technical Decisions | Core team             | 2 years  | Ship quickly        |
| Marketing           | Dedicated team        | Ongoing  | Drive adoption      |
| Partnerships        | Business development  | Ongoing  | Enterprise adoption |
| Documentation       | Technical writers     | Ongoing  | Developer success   |

**Sunset Provisions**:
- Foundation voting power decreases 20% yearly
- Development fund transitions to DAO control
- Technical decisions shift to governance
- All special powers expire by year 5

### Appendix C: Success Stories We Want

**Year 1**: “Startup Raises $5M Using `.mystartup` TLD”

- Company uses `.mystartup` domain for all properties
- Investors see innovation mindset
- Media coverage drives Dap awareness

**Year 2**: “Fortune 500 Migrates to `.mybrand` TLD”

- Major corporation adopts Dap for brand protection
- Demonstrates enterprise viability
- Drives institutional adoption

**Year 3**: “Developer Earns $1M from Domain App”

- Individual developer builds successful service
- Proves ecosystem economic opportunity
- Attracts more builders

**Year 5**: “Dap Serves 1 Billion DNS Queries Daily”

- Achieving scale comparable to major DNS providers
- Utility at global scale
- Undeniable product‑market fit

### Appendix D: The Anti‑Patterns We Avoid

**Governance Paralysis**: Other projects spent months debating minor parameter changes while shipping nothing. We decide in days and iterate.

**Purity Spirals**: Other communities attacked any pragmatism as betrayal. We celebrate what works.

**Technical Superiority Without Usage**: Others built “the best” system nobody uses. We build good‑enough systems millions use.

**Community Gatekeeping**: Toxic maximalism drove away builders. We welcome anyone who ships.

**Speculation Over Utility**: Others optimized for token price over product development. We optimize for usage metrics.

**Documentation Negligence**: Others never properly documented APIs or tools. We maintain comprehensive, updated documentation.

**User Hostility**: Others expected users to understand blockchain complexity. We hide complexity behind simple, intuitive interfaces.

**ICANN Deference**: Others reserved ICANN namespaces out of misplaced respect. We compete on merit.

---

*Join us: [https://dap.sh](https://dap.sh)*

*Version 9*
