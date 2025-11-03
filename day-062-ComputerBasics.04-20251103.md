# Day 62: Browsing the web effectively

## Key topics covered:
- [x] common web browsers
- [x] web browser, website and search engine
- [x] how to use search engine effectively

## 1. 
You can install a browser through your operating system's package manager, such as `brew install --cask google-chrome` on macOS with Homebrew, or `yay -S brave-bin` on Arch Linux.

The package manager and package names available to you will vary depending on your operating system.

## 2.
### 2.1 Web browser
Web browsers are software applications that allow users to access and navigate the World Wide Web. 

Key features of web browsers include the address bar, where you enter URLs or search queries, and the rendering engine, which translates HTML, CSS, and JavaScript into visual web pages.

**Popular web browsers: Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, and Opera.**

### 2.2 Website
Collections of web pages and related content that are identified by a common domain name and published on at least one web server. They are the destinations you visit using your web browser.

Components of websites:
- domain name
- web pages

Websites can be
- static: where content rarely changes
- dynamic: where content updates frequently or is personalized for users.

### 2.3 Search Engine
Web-based tools designed to help users find information on the internet. They use complex algorithms to index and rank web pages based on relevance to user queries.

Key aspects of search engines
- web crawlers (aka spiders or bots): programs that systematically browse the web to discover and index new content.
- ranking algorithm: complex systems that determine the order of search results based on factors like relevance, authority, and user experience

**Popular search engines: Google, Bing, Yahoo, and DuckDuckGo.**

---

The relationship between browsers, websites, and search engines is interconnected.
| Item | WHat it does |
| --- | --- |
| **Web browsers **| tools used to access both websites and search engines |
| **Websites**| the destinations that users visit through browsers or find via search engines |
| **Search engines** | help users discover websites by providing organized access to the vast amount of information on the web |

## 3. how to use search engine effectively
Boolean search syntax
- Example 1: `freecodecamp curriculum`  - the search engine will return results that match any of these keywords
- Example 2: `"freecodecamp curriculum"` - results you will see will be limited to sites that say freecodecamp curriculum together, not sites that say freecodecamp AND curriculum.
- Example 3: `+freecodecamp +curriculum` - match sites that include both of those terms, but not necessarily next to each other as a phrase
- Example 4: `+freecodecamp -curriculum` - return results that mention freecodecamp, but exclude results that also mention curriculum.
- Example 5: `site:freecodecamp.org/news curriculum.` - search a specific site that contain the word `curriculum`.

Super example: `site:freecodecamp.org/news +python -curriculum` would search for Python articles on our news site, excluding articles that might talk about our curriculum.

[Ends 21:18 3 Nov 2025]
