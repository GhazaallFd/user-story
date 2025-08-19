<summary><h1 style="display: inline-block;border: none">Story</h1></summary>

## 📝 STEP 1

Property extraction:

|          Field           | Required |                                Description                                |
| :----------------------: | :------: | :-----------------------------------------------------------------------: |
|     News Title     |    ✅    |                    The headline of the news article.                         |
|      Topic Tags      |    ✅    |                      Keywords or tags linked to trending topics (e.g. "قیمت طلا", "ایران‌خودرو").                        |
|    Publish Date      |    ✅    | The date and time the news article was originally published (used for tie-break if two articles have the same view count). |
| Visit Count |    ✅    |             The number of total views the article has received (used to determine the top 5 most-viewed articles in the last 6 hours).            |
| Thumbnail Image |    ✅    |            A visual preview image for use in story format.             |
| Source Name |    ✅    |            The name of the media outlet that published the article (e.g. خبرفوری, ایلنا).           |
| Source Logo |    ❌ (optional)    |             The logo or icon of the source, used for branding within the story.           |
| Display Duration |    ✅    |             The number of seconds the story stays visible before switching (e.g. 7s).           |
| Viewer Status |    ✅    |             Indicates if the current user has seen the story (seen / unseen).            |
| Expiration Time |    ✅    |            The story should stop being shown after the 6-hour window ends (when the top 5 refresh).          |
| User Reaction |    ❌ (optional)   |             The reaction given by the user to the story (e.g. ❤️, 👎, 😐) – optional.             |

## 📝 STEP 2

Behavioral Acceptance Criteria:

|          Feature           | Priority |                                Acceptance Criteria (AC)                                |
| :----------------------: | :------: | :-----------------------------------------------------------------------: |
|     Auto-play stories     |    High    |                 Each story should automatically move to the next one after a defined duration (e.g., 7 seconds).                        |
|      Manual navigation     |    High    |                      The user should be able to navigate back or forward by tapping/clicking left or right.                       |
|    Seen/Unseen indicator      |    High    | Stories the user has already viewed must be visually distinguished (e.g., dimmed, full progress bar). |
| Resume position |    Medium    |             If the user exits mid-story, they should resume from the same point when returning, not from the beginning.           |
| Expiration handling |    High    |         Stories must automatically expire and refresh every 6 hours, showing the latest top 5 most-viewed articles per source.        |
| Pause/Resume |    Medium    |            The user should be able to pause a story by holding (tap & hold) and resume by releasing.           |
| Story prioritization |   High    |           Exactly 5 most-viewed articles from each source (within the last 6 hours) must be shown, sorted by Visit Count (desc) and then by Publish Date (desc).
| User reactions |    Medium    |             Users should be able to react to stories with quick emoji responses; reactions must be saved instantly.          |
| Source navigation |    High    |            The user must be able to click on the source name/logo and be redirected to the news source’s main page.           |
| Cross-source continuity |    Medium    |          After finishing all 5 stories from one source, the next source’s stories should play seamlessly.    |
| Progress indicator |    High    |          Each story must have a progress bar showing remaining time and total number of stories (always 5).            |
| Passive consumption |High   |      Without any interaction, the system must auto-play all 5 stories in sequence.        |
| Mobile/Desktop support |High   |        Stories must be fully functional on both mobile (gesture-based) and desktop (click/keyboard) environments, always showing 5 stories per source.         |
## 📝 STEP 3

**Description**

The goal of the Story feature is to provide users with quick access to each source’s top news. The Story section displays the top 5 most-viewed articles per source, refreshed every 6 hours, with the same stories shown consistently on both mobile and desktop. Stories are ordered by Visit Count (descending), and in case of ties, by Publish Date (descending).

## 📝 STEP 4

1. As a user, I want to see the title of each news article in the story, so that I can quickly understand the main topic before reading more.
<br />
<br />

2. As a user, I want stories to be grouped by source, showing the top 5 most-viewed articles for that source in the last 6 hours, so that I can catch up quickly.
<br />
<br />

3. As a user, I want to know how recent each news article is, so that I can decide whether the information is still relevant.
<br />
<br />

4. As an admin, I want to track article views (and compute the “top 5 in the last 6 hours”), so that the Story set is always based on accurate popularity data.
<br />
<br />

5. As a user, I want each story item to include a visual thumbnail, so that the content feels more engaging and helps me understand the news at a glance.
<br />
<br />

6. As a user, I want to see the name and logo of the news source with each article, so that I know where the information is coming from and can judge its credibility.
<br />
<br />

7. As a user, I want each story to stay on screen for a few seconds before automatically moving to the next, so that I can view the content comfortably without needing to interact manually.
<br />
<br />

8. As a user, I want to know which stories I have already viewed (seen/unseen), so that I can focus only on the new or unseen stories.
<br />
<br />


9. As an admin, I want the system to always present exactly five stories per source on both mobile and desktop, so that the experience is consistent.
<br />
<br />


10. As a user, I want stories to automatically expire after 6 hours and be replaced by the newly computed top 5, so that I always see the most current popular content.
<br />
<br />

11. As a user, I want to be able to react to story items using emojis, so that I can quickly express my opinion without leaving the story.
<br />
<br />

12. As a user, I want the same five stories and the same order on mobile and desktop, so that my experience is consistent across devices.
<br />
<br />

13. As a user, I want the stories within a source ordered by most-viewed first, and when two items have the same views, the newer one should appear earlier.
<br />
<br />