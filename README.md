**Smart IMDb Ratings Update - Metadata Repair & Synchronization**
===============================================================

Smart IMDb Ratings Update is an advanced Kodi add-on designed to automatically maintain and repair your Kodi video library metadata.
Originally created as an independent evolution inspired by Light IMDb Ratings Update, the project has grown into a comprehensive metadata maintenance engine that not only updates IMDb ratings, but also repairs incomplete metadata, synchronizes identifiers, updates TV show statuses, and keeps IMDb Top 250 information current.
Unlike the original add-on, which provides only basic rating updates, Smart IMDb Ratings Update focuses on automation, resilience, and intelligent metadata recovery, ensuring that incomplete or outdated library information is automatically corrected whenever possible.


**Key Features**
==============
Rating Updates
1. Automatic rating updates after Kodi library scans (new items only)
2. Optional Monthly Full Refresh for ratings on the entire Kodi library
3. Late-publication period for extending dataset monitoring window when IMDb publishes dataset later than expected
4. Context menu updates with selectable source:
 a) api.tiffara.com
 b) Local IMDb Dataset (official IMDb non-commercial datasets)
 c) IMDb HTML (currently retained for compatibility; direct HTML retrieval is blocked by Cloudflare)

Metadata Recovery
1. Automatic recovery of missing IMDb, TMDB and TVDB identifiers
2. Automatic repair of incorrect or incomplete identifiers
3. Intelligent multi-stage recovery engine using IMDb, TMDB and TVDB
4. Automatic writing of recovered identifiers back into the Kodi database
5. Complete recovery support for Movies, TV Shows, Seasons and Episodes
6. Episode rating resolution even when episode-level IMDb IDs are initially unavailable
7. Multiple recovery paths for episode identifiers, including TV Show -> Episode derivation

Metadata Synchronization
1. Automatic synchronization of TV Show status from TMDB (optional)
2. IMDb Top 250 synchronization (optional)
3. Automatic TV show banner recovery from TVDB (optional)

Performance & Reliability
1. Local IMDb Dataset support for extremely fast offline rating updates
2. Built-in API rate limiting
3. Daily logging with automatic log rotation
4. Persistent logging across Kodi and add-on restarts
5. Integrated log viewer displaying the latest activity directly from the add-on
6. Extensive protection against incomplete metadata, missing datasets and API failures

IMDb Top 250 Support
Top250 information may be obtained from one of the following sources:
1. Local Top250.txt file placed manually inside the add-on's /db directory.
2. Top250.txt generated automatically by the companion Python utility available on my GitHub (recommended for scheduled synchronization).
3. top250.info/charts, updated daily (used with permission from the website owner).


**Philosophy**
============
The goal of this project is metadata accuracy, resilience and self-healing.
Instead of silently skipping items with incomplete metadata, the add-on attempts multiple recovery strategies to reconstruct missing information using relationships available across IMDb, TMDB and TVDB.
As a result, Smart IMDb Ratings Update does considerably more than update ratings - it continuously improves the overall quality of your Kodi library by repairing identifiers, synchronizing metadata and keeping important information up to date.
The project has been extensively tested against numerous real-world edge cases and is designed to operate reliably even with partially incomplete libraries.


**Important Notes**
=================
This add-on updates metadata stored in your Kodi library.
Although it has been designed with reliability in mind, creating a backup of your Kodi database before first use is strongly recommended.
The project is considered feature complete. Future development will primarily focus on compatibility updates required by changes in Kodi, IMDb, TMDB or TVDB services.

**Credits**
=========
This project was originally inspired by Light IMDb Ratings Update, but has since evolved into a substantially redesigned solution featuring intelligent metadata recovery, automatic identifier repair, advanced scheduling, TV Show metadata synchronization and comprehensive fallback mechanisms.
