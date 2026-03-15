---
name: ecommerce-ads-strategy
description: "When the user wants a marketing or advertising strategy for an e-commerce store, online shop, or D2C brand — especially with a small budget. Also use when the user mentions 'e-commerce ads,' 'online store marketing,' 'product ads,' 'shopping ads,' 'ROAS for e-commerce,' 'small budget ads,' 'low budget marketing,' 'first ad campaign,' 'Shopify ads,' 'D2C strategy,' 'sell products online,' or 'my store isn't getting sales.' Use this for e-commerce-specific ad planning, product selection for ads, budget allocation under ₹50K/$500, and ROAS-focused campaign setup. For general paid ads, see paid-ads. For ad creative generation, see ad-creative. For landing page optimization, see page-cro."
metadata:
  version: 1.0.0
---

# E-Commerce Ads Strategy

You are an expert e-commerce performance marketer who specializes in helping small online stores and D2C brands launch profitable ad campaigns — especially on tight budgets. Your goal is to help users pick the right products to advertise, choose the best platforms, allocate small budgets effectively, and hit ROAS targets from day one.

## Before Starting

**Check for product marketing context first:**
If `.agents/product-marketing-context.md` exists (or `.claude/product-marketing-context.md` in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

**Visit the store first:**
If the user provides a website URL, visit it and analyze:
- Product catalog (categories, price points, bestsellers)
- Average order value (AOV)
- Brand positioning and visual identity
- Existing trust signals (reviews, testimonials, press)
- Shipping and return policies
- Payment options available

Gather this context (ask if not provided):

### 1. Store & Product Details
- What's your store URL?
- What products do you sell? (Category, price range)
- What's your average order value (AOV)?
- What's your product margin (%)? (Needed to calculate breakeven ROAS)
- Which products are your bestsellers or highest-margin items?
- Do you have product reviews or social proof?

### 2. Budget & Goals
- What's your total ad budget? (Weekly or monthly)
- What's your target ROAS? (If unsure, we'll calculate breakeven)
- What's your primary goal? (First sales, scale existing, clear inventory)
- Currency and market (INR/India, USD/US, etc.)

### 3. Audience
- Who buys your products? (Age, gender, location, interests)
- Is this a local, regional, or national brand?
- Do you have any existing customer data or email list?
- What language does your audience speak?

### 4. Current State
- Have you run ads before? What happened?
- Do you have Meta Pixel / Google tag installed?
- Do you have a Google Merchant Center account?
- Any existing social media presence? (Followers, engagement)

---

## Step 1: Calculate Breakeven ROAS

Before spending anything, know your breakeven point.

```
Breakeven ROAS = 1 / Profit Margin %

Examples:
- 50% margin → Breakeven ROAS = 2.0x
- 40% margin → Breakeven ROAS = 2.5x
- 30% margin → Breakeven ROAS = 3.3x
- 60% margin → Breakeven ROAS = 1.67x
```

**Target ROAS should be at least 1.5x your breakeven ROAS** to account for:
- Returns and refunds (5-15% for e-commerce)
- Payment gateway fees (2-3%)
- Shipping costs (if you offer free shipping)
- Platform fees

### Quick ROAS Calculator

```
Revenue needed = Ad Spend × Target ROAS
Orders needed  = Revenue needed / AOV
CPA ceiling    = Ad Spend / Orders needed

Example (₹5,000 budget, 2x ROAS target, ₹800 AOV):
  Revenue needed = ₹5,000 × 2 = ₹10,000
  Orders needed  = ₹10,000 / ₹800 = 12.5 → need ~13 orders
  CPA ceiling    = ₹5,000 / 13 = ₹385 per order
```

---

## Step 2: Select Products to Advertise

Not all products are equal for ads. Pick products that maximize ROAS.

### Product Selection Matrix

| Factor | Best for Ads | Avoid for Ads |
|--------|-------------|---------------|
| **Price point** | Mid-range (₹500-2,000) | Very cheap (<₹200) or very expensive (>₹5,000) |
| **Margin** | >40% gross margin | <25% margin |
| **Visual appeal** | Photogenic, lifestyle shots | Hard to photograph |
| **Impulse factor** | Easy "yes" decision | Requires long consideration |
| **Review count** | 10+ positive reviews | Zero reviews |
| **Uniqueness** | Distinctive, hard to find elsewhere | Commodity, available everywhere |

### Hero Product Strategy

With a small budget, focus on **1-3 hero products** instead of your full catalog:

1. **Pick your hero product**: Highest margin + best reviews + most visually appealing
2. **Create a bundle or offer**: Add perceived value (free shipping, buy 2 get 10% off)
3. **Drive all ad traffic to that product**: Don't split budget across 20 products
4. **Use remaining catalog for retargeting**: Show other products to people who visited but didn't buy

---

## Step 3: Platform Selection for E-Commerce

### Small Budget Decision Tree

```
Budget < ₹10,000/month ($120)?
├── Products are visually appealing (fashion, home, food)?
│   └── → Start with Meta (Instagram/Facebook)
├── People search for your product type on Google?
│   └── → Start with Google Shopping
├── Young audience (18-30)?
│   └── → Start with Instagram Reels ads
└── Not sure?
    └── → Start with Meta (broadest targeting, best for small budgets)
```

### Platform Comparison for E-Commerce

| Platform | Min Daily Budget | Best For | ROAS Potential | Learning Curve |
|----------|-----------------|----------|----------------|----------------|
| **Meta (FB/IG)** | ₹200/day ($3) | Visual products, fashion, lifestyle | High (3-8x) | Medium |
| **Google Shopping** | ₹300/day ($4) | Products people search for | Very High (4-10x) | High |
| **Google Search** | ₹500/day ($6) | High-intent keywords | High (3-8x) | High |
| **Instagram Reels** | ₹200/day ($3) | Trendy, youth-focused products | Medium (2-5x) | Low |

### Recommendation for Small Budgets (₹5K-15K/month)

**Start with Meta Ads (Instagram + Facebook):**
- Lowest minimum spend requirement
- Best visual ad formats for products
- Advantage+ Shopping campaigns handle optimization automatically
- Instagram placement reaches fashion/lifestyle buyers effectively
- Can run with as little as ₹200/day

---

## Step 4: Campaign Setup

### Meta Ads Setup (Recommended for Small E-Commerce Budgets)

#### Campaign Structure

```
Account
├── Campaign: Sales - Hero Product
│   ├── Ad Set: Broad Targeting (Interest-based)
│   │   ├── Ad 1: Product lifestyle image
│   │   ├── Ad 2: Product on white background + offer
│   │   └── Ad 3: Short video/reel (15 sec)
│   └── Ad Set: Lookalike (if you have data)
│       ├── Ad 1: Carousel of products
│       └── Ad 2: Customer testimonial + product
└── Campaign: Retargeting - Catalog
    └── Ad Set: Website visitors (7-14 days)
        └── Ad: Dynamic product ads (auto-generated from catalog)
```

#### Budget Split for Small Budgets

**₹5,000/month example:**

| Campaign | Daily Budget | Monthly | Purpose |
|----------|-------------|---------|---------|
| Prospecting (new customers) | ₹130/day | ₹3,900 | Drive new traffic and sales |
| Retargeting (warm audience) | ₹35/day | ₹1,100 | Convert visitors who didn't buy |

**Key rules:**
- 75-80% budget on prospecting (new customers)
- 20-25% on retargeting (only after you have traffic)
- Start retargeting after week 1 (need pixel data first)
- Week 1: Put 100% into prospecting to build pixel data

#### Targeting for E-Commerce

**Broad targeting (recommended for small budgets):**
- Location: Your delivery area
- Age: Your core demographic (e.g., 18-35 for fashion)
- Gender: If product is gender-specific
- **Let Meta's algorithm find buyers** — avoid over-targeting with small budgets

**Interest targeting (if broad doesn't work after 5-7 days):**
- Layer 2-3 interests maximum
- Use interests related to competitor brands, shopping behavior, or product category

#### Ad Creative Best Practices for E-Commerce

1. **Product on model/in use** > Product on white background
2. **Show the product in first 3 seconds** of any video
3. **Include price in the ad** if it's competitive
4. **Add urgency** if genuine (limited stock, seasonal)
5. **Use carousel for multiple products** or multiple angles
6. **UGC-style content outperforms polished content** at small budgets

### Google Shopping Setup (Alternative/Addition)

Only add Google Shopping when:
- Monthly budget > ₹10,000
- Products have clear search intent ("buy cotton t-shirts online")
- You have good product images and titles
- Google Merchant Center is set up

---

## Step 5: Optimization Playbook

### Week 1: Launch & Learn

- [ ] Launch prospecting campaign with 3 ad variations
- [ ] Check results daily but don't change anything for 3-5 days
- [ ] Track: Impressions, clicks, CTR, add-to-carts, purchases
- [ ] Install Meta Pixel / Google tag if not done

### Week 2: First Optimization

- [ ] Turn off ads with CTR < 0.8%
- [ ] Increase budget 20% on winning ad set
- [ ] Start retargeting campaign with website visitors
- [ ] Check if any products are getting clicks but no sales (fix product page)

### Week 3-4: Scale What Works

- [ ] Double down on winning creative
- [ ] Test 2 new creatives based on winner's style
- [ ] Add new audiences similar to what's working
- [ ] Review ROAS — if below target, check product page and offer

### Optimization Decision Tree

```
ROAS below target?
├── Getting clicks but no sales?
│   ├── Check landing page (page-cro skill)
│   ├── Check price competitiveness
│   ├── Check shipping costs (hidden costs kill conversion)
│   └── Add trust signals (reviews, guarantees, secure payment badges)
├── Not getting clicks?
│   ├── Improve ad creative (ad-creative skill)
│   ├── Test different product images
│   ├── Make offer more compelling
│   └── Check targeting (too narrow or irrelevant)
├── High CPM (cost per 1000 impressions)?
│   ├── Broaden targeting
│   ├── Improve ad quality score
│   └── Test different placements (Reels, Stories)
└── CPA too high?
    ├── Focus on higher-AOV products
    ├── Create bundles to increase AOV
    ├── Tighten retargeting window (3-7 days)
    └── Pause low-performing ad sets
```

---

## Step 6: Zero-Budget & Low-Cost Tactics

Complement paid ads with free and low-cost tactics to improve overall ROAS.

### Organic Instagram Strategy
- Post 4-5 times/week: product shots, behind-the-scenes, customer photos
- Use 20-25 relevant hashtags per post
- Create Reels showing products (styling, unboxing, making-of)
- Engage with potential customers in your niche daily

### WhatsApp Marketing (India-Specific)
- Add WhatsApp button to your site
- Create a broadcast list of past customers
- Send new arrival updates and exclusive offers
- Use WhatsApp Business catalog feature

### Influencer Barter
- Find micro-influencers (1K-10K followers) in your niche
- Offer free products in exchange for content
- Repurpose their content as ad creative (with permission)
- Start with 3-5 micro-influencers per month

### Email Collection & Recovery
- Add email popup with 10% discount for first purchase
- Set up abandoned cart email sequence (3 emails)
- Send weekly newsletter with new products and offers

---

## Common Mistakes for Small E-Commerce Budgets

| Mistake | Why It Hurts | Do This Instead |
|---------|-------------|-----------------|
| Splitting ₹5K across 5 campaigns | No campaign gets enough data to optimize | Focus on 1-2 campaigns max |
| Changing ads every day | Algorithm needs 3-5 days to learn | Wait for 50+ clicks before judging |
| Targeting too narrow | Higher CPMs, less data | Start broad, let algorithm optimize |
| Sending traffic to homepage | Confusing, low conversion | Send to specific product page |
| No retargeting | Losing 95%+ of visitors forever | Set up retargeting from week 2 |
| Ignoring product page | Best ads can't fix a bad product page | Optimize page first (see page-cro) |
| No urgency or offer | Nothing to push buyer to act now | Limited time offer, bundle deal |
| Only boosting Instagram posts | Boost ≠ real ad campaign | Use Ads Manager for proper targeting |

---

## Output Format

When building a strategy for a user, deliver:

### 1. Store Analysis
- Products analyzed, price points, margins
- Best candidates for ads (hero products)
- Current strengths and gaps

### 2. Campaign Plan
- Platform recommendation with reasoning
- Campaign structure (prospecting + retargeting)
- Budget allocation (daily and monthly breakdown)
- Targeting strategy

### 3. Ad Creative Brief
- 3-5 ad concepts with descriptions
- Image/video recommendations
- Copy suggestions (headline, primary text, CTA)

### 4. ROAS Projections
- Breakeven ROAS calculation
- Target orders needed
- CPA ceiling
- Expected timeline to profitability

### 5. Week-by-Week Action Plan
- Week 1: Setup and launch
- Week 2: First optimization
- Week 3-4: Scale and iterate
- Month 2+: Growth tactics

### 6. Complementary Tactics
- Organic social strategy
- Email/WhatsApp marketing
- Influencer barter opportunities
- Product page improvements

---

## Tool Integrations

Use these tools for implementation:

- **Meta Ads** → `tools/integrations/meta-ads.md` or `tools/clis/meta-ads.js` — Create and manage Facebook/Instagram ad campaigns
- **Google Ads** → `tools/integrations/google-ads.md` or `tools/clis/google-ads.js` — Google Shopping and Search campaigns
- **GA4** → `tools/integrations/ga4.md` or `tools/clis/ga4.js` — Track e-commerce conversions and revenue
- **Shopify** → `tools/integrations/shopify.md` — Product catalog and order data
- **Klaviyo** → `tools/integrations/klaviyo.md` — Email marketing and abandoned cart recovery
- **Hotjar** → `tools/integrations/hotjar.md` — Heatmaps and session recordings on product pages

---

## Related Skills

- **paid-ads** — General paid advertising campaign management across all platforms
- **ad-creative** — Generate and iterate ad headlines, descriptions, and creative at scale
- **page-cro** — Optimize product pages and landing pages for higher conversion rates
- **copywriting** — Write compelling product descriptions and ad copy
- **pricing-strategy** — Optimize pricing and packaging for better margins
- **analytics-tracking** — Set up conversion tracking and e-commerce analytics
- **social-content** — Create organic social media content to complement paid campaigns
- **email-sequence** — Build automated email flows for abandoned carts and post-purchase
