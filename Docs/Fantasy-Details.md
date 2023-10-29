# FLI GOLF Fantasy League

Get ready for a Disc Golf revolution unlike anything you've ever seen before! FLI GOLF League proudly stands as the pioneer of fantasy-style exhibition tournaments in the history of Disc Golf.

**The Concept:**

- Six electrifying teams
- 36 powerhouse players
- A fantasy format that will blow your mind!

FLI Fantasy pits teams against each other, whether it's the epic clash of **TEAMS VS. TEAMS** or the thrilling showdown of **PLAYERS VS. PLAYERS**. In this exhilarating battle, the team with the lowest total score snatches not only victory but also **THE PRIZE**!

## How it Works

1. **Registration:**
   Six eager players register their league on [FLIGOLF.COM](http://FLIGOLF.COM).
2. **Draft Order & Matchups:**
   Two days before the tournament, the draft order and matchups are randomly generated.
3. **Drafting:**
   A snake-style draft takes place over six rounds. The first four rounds see teams selecting their top men, women, or FLI GOLF teams. The final two rounds are dedicated to securing backup players.
4. **The Tournament:**
   With two men, two women, and backup players ready, the tournament goes live on the FLI GOLF Fantasy app. Watch in real-time as the team with the lowest total score claims victory.

**Prizes:**

- Cash
- Prestige
- Exclusive FLI GOLF gear worth up to $1,200

**Special Prizes:**

- College logo/FLI Golf logo collaboration shirts

## Scoring Explanation

1. **Matchups:**
   Each tournament will have three matchups that are randomly generated after the draft order is set. The lowest total teams or players scores win the 1 on 1 matchup. Each league will have three winners per tournament.
2. **Points:**
   - Each legal throw counts as 1 point.
   - Shots over par record a 2x outcome.
     - Bogie adds 2 points to the team score.
     - Double bogie adds 4 points to the team score.
   - Shots under par drop 0.5 points off the total team score, per under par position.
3. **Examples:**
   - A birdie on a par 3 will record 1.5 strokes instead of 2.
   - A hole-in-one on a par 3 will record "0" on the scorecard.

\*All regular scoring rules apply to teams that have replacement players moved to an active position for a tournament.

## Join the Revolution

This is what the world has been waiting for—the interactive Disc Golf experience sports books dream about! For just $300 per league for the entire year, it's your ticket to an adrenaline-packed adventure without breaking the bank. Disc Golf enthusiasts, this is your moment! Join us, embrace the thrill, and let FLI GOLF Fantasy redefine the way you experience your favorite sport!

# Fantasy Feature Implementation Workflow

## Step 1 Subscription Payment

1. Integrate Stripe for handling subscription payments.
2. Post-payment, update user's role in `profiles` table to "Subscriber".

## Step 2: Drafting Process

1. Develop a UI for users to participate in the draft.
2. Allow users to select players from the `pros` table during the draft.
3. Save drafted teams in a new table or update the existing `teams` table.

## Step 3: Tournament Scoring

1. Develop a UI to display live tournament scores.
2. Utilize `scores` table to calculate scores for each player and team.
3. Update UI in real-time as scores are updated.

## Step 4: Award Prizes

1. Post-tournament, determine winners based on scores.
