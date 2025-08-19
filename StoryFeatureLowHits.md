<summary><h1 style="display: inline-block;border: none">Story</h1></summary>

## 📝 STEP 1

Property extraction:

|          Field           | Required |                                Description                                |
| :----------------------: | :------: | :-----------------------------------------------------------------------: |
|     News Title     |    ✅    |                    The headline of the news article.                         |
|      Topic Tags      |    ✅    |                      Keywords or tags linked to trending topics (e.g. "قیمت طلا", "ایران‌خودرو").                        |
|    Publish Date      |    ✅    | The date and time the news article was originally published. |
| Visit Count |    ✅    |             The number of total views the article has received.            |
| Thumbnail Image |    ✅    |            A visual preview image for use in story format.             |
| Source Name |    ✅    |            The name of the media outlet that published the article (e.g. خبرفوری, ایلنا).           |
| Source Logo |    ❌ (optional)    |             The logo or icon of the source, used for branding within the story.           |
| Display Duration |    ✅    |             The number of seconds the story stays visible before switching (e.g. 7s).           |
| Viewer Status |    ✅    |             Indicates if the current user has seen the story (seen / unseen).            |
| Max View Limit |    ✅    |            The maximum number of views allowed via the story (e.g. 200 views).             |
| Expiration Time |    ✅    |            The time at which the story should stop being shown (e.g. 24 hours after start).            |
| User Reaction |    ❌ (optional)   |             The reaction given by the user to the story (e.g. ❤️, 👎, 😐) – optional.             |

## 📝 STEP 2

Behavioral Acceptance Criteria:

|          Feature           | Priority |                                Acceptance Criteria (AC)                                |
| :----------------------: | :------: | :-----------------------------------------------------------------------: |
|     Auto-play stories     |    High    |                 Each story should automatically move to the next one after a defined duration (e.g., 7 seconds).                        |
|      Manual navigation     |    High    |                      The user should be able to navigate back or forward by tapping/clicking left or right.                       |
|    Seen/Unseen indicator      |    High    | Stories the user has already viewed must be visually distinguished (e.g., dimmed, full progress bar). |
| Resume position |    Medium    |             If the user exits mid-story, they should resume from the same point when returning, not from the beginning.           |
| Expiration handling |    High    |            Story loading time should be under 2 seconds for a seamless user experience.             |
| Pause/Resume |    Medium    |            The user should be able to pause a story by holding (tap & hold) and resume by releasing.           |
| Story prioritization |   High    |             Stories must be prioritized and displayed according to defined rules (e.g., low-visibility or trending-tag news).           |
| User reactions |    Medium    |             Users should be able to react to stories with quick emoji responses; reactions must be saved instantly.          |
| Source navigation |    High    |            The user must be able to click on the source name/logo and be redirected to the news source’s main page.           |
| Cross-source continuity |    Medium    |           After finishing all stories from one source, the next source’s stories should play seamlessly           |
| Progress indicator |    High    |            Each story must have a progress bar showing remaining time and total number of stories.            |
| Passive consumption |High   |        Without any interaction, the system must auto-play all available stories in sequence.         |
| Mobile/Desktop support |High   |        Stories must be fully functional on both mobile (gesture-based) and desktop (click/keyboard) environments.         |
## 📝 STEP 3

**Description**

The goal of the Story feature is to increase the visibility of fresh, low-view news articles.
Instead of focusing only on the most-viewed content, we’re introducing a Story section that highlights lesser-seen news related to trending topics, presented in  engaging format.

## 📝 STEP 4

1. As a user,
I want to see the title of each news article in the story,
So that I can quickly understand the main topic before reading more.
<br />
<br />

2. As a user,
I want stories to be grouped and shown based on trending topic tags,
So that I can easily find news that matches my current interests.
<br />
<br />

3. As a user
I want to know how recent each news article is,
So that I can decide whether the information is still relevant.
<br />
<br />

4. As an admin,
I want to track how many views each article has received,
So that I can manage which articles should be promoted or replaced in the Story section.
<br />
<br />

5. As a user,
I want each story item to include a visual thumbnail,
So that the content feels more engaging and helps me understand the news at a glance.
<br />
<br />

6. As a user,
I want to see the name and logo of the news source with each article,
So that I know where the information is coming from and can judge its credibility.
<br />
<br />

7. As a user,
I want each story to stay on screen for a few seconds before automatically moving to the next,
So that I can view the content comfortably without needing to interact manually.
<br />
<br />

8. As a user,
I want to know which stories I have already viewed,
So that I can focus only on the new or unseen stories.
<br />
<br />


9. As an admin,
I want to set a view limit for each story,
So that low-visibility news can rotate out after reaching a fair exposure level.
<br />
<br />


10. As a user,
I want stories to automatically disappear after a fixed time (like 24 hours),
So that I always see only the most recent and relevant content.
<br />
<br />

11. As a user,
I want to be able to react to story items using emojis,
So that I can quickly express my opinion without leaving the story.
<br />
<br />
