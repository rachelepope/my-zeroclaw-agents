# SKILL 1: Intelligence Acquisition & Alignment
**Trigger:** The user sends a [Keyword] or [Topic] via Telegram.

**Execution Protocol:**
1. **Search:** Invoke web_search_tool to gather the latest data on the 
   [Keyword], with a priority focus on:
   - Banking, fintech, NBFIs, asset managers, and insurance sectors
   - Abu Dhabi and UAE market developments
   - IHC shareholder announcements and related entities
   - Regional and global developments that impact UAE financial services

2. **Synthesise & Align:** Filter through the 'Super Individual' lens. 
   Answer: how does this serve a small, fast-moving financial services 
   team in Abu Dhabi that is eager to grow fast?

3. **Format the Output:** Reply via Telegram in this exact structure:
   - **TL;DR:** one-sentence summary.
   - **The Leverage:** why this matters for a UAE financial services team.
   - **Integration Idea:** one practical way to act on this intelligence.

4. **Archive:** Use file_write to save the summary as a Markdown file in
   /root/.zeroclaw/workspace/luna/archive/
   Naming convention: YYYY-MM-DD_[Keyword].md

# SKILL 2: The Weekly Synthesis
**Trigger:** User command, or weekend automated trigger.

**Execution Protocol:**
1. **Retrieve:** Use file_read to read all .md files saved in
   /root/.zeroclaw/workspace/luna/archive/ over the last 7 days.
2. **Synthesise:** Identify overlaps, trends, and key developments 
   across UAE banking, fintech, NBFIs, asset managers, and insurance.
3. **Deliver:** A 'Weekly Intelligence Report' summarising strategic 
   takeaways for a UAE financial services team.
4. **Save:** /root/.zeroclaw/workspace/luna/weekly/
   Naming: YYYY-MM-DD-Weekly.md
