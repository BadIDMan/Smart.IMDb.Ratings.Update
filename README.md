Smart IMDb Ratings Update
=========================
Smart IMDb Ratings Update is an advanced Kodi add-on for automatically updating movie, TV show, and episode ratings using multiple data sources with intelligent fallback logic.</br>
This project was created as an independent evolution inspired by Light IMDb Ratings Update.</br>
While the original add-on provides a very minimal implementation (for example, limited scheduling options and no fallback mechanisms), this version focuses on reliability, automation, and self-healing rating updates across the entire library.

Key Features
============
1. Automatic rating updates after Kodi library scans (new items only)
2. Context menu updates with selectable source:</br>
a) IMDbAPI.dev</br>
b) Local IMDb dataset (official IMDb non-commercial datasets)</br>
c) IMDb HTML (currently blocked by WAF protection so API calls fails)</br>
3. Full support for Movies, TV Shows, and Episodes
4. Intelligent multi-stage fallback system: IMDb -> TMDB -> TVDB -> ID recovery
5. Automatic recovery and writing of missing IDs back to Kodi
6. Episode rating resolution even when episode-level IMDb IDs are missing
7. Local dataset support for fast, offline rating updates
8. Built-in rate limiting for API usage
9. Detailed logging with in-app log viewer (last 20 lines)
10. Protection against missing dataset and edge-case failures

Philosophy
==========
The goal of this add-on is accuracy and resilience.</br>
Instead of failing silently or skipping items when data is incomplete, the engine attempts multiple resolution strategies to ensure ratings are populated whenever possible.</br>
This includes recovering missing identifiers, resolving conflicts, and using alternative data sources when needed.</br>
The add-on has been heavily tested against many edge cases, and is designed to be stable and reliable across a wide range of real-world library scenarios.</br>

Important Notes
===============
This add-on is provided as-is.</br>
It will not be maintained, except in cases where external changes (e.g. API changes, Kodi changes) completely break its functionality.</br>
The add-on does not support IMDb Top250 updates for movies (this feature was intentionally omitted).</br>
The author takes no responsibility for any damage to the Kodi database -> it is strongly recommended to create a backup before using this add-on.</br>

Credits
=======
This project was inspired by Light IMDb Ratings Update, but has been significantly redesigned and extended to address limitations such as lack of fallback logic, minimal scheduling capabilities, and limited update scope.
