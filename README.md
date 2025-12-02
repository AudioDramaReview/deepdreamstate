Deep Dream State - Metadata Repository
Structured metadata for the Deep Dream State audio drama series in JSON format.
Directory Structure
/data/
  /show/
    metashow.json
  /episodes/
    arc1-episode-001.json
    arc1-episode-002.json
    arc1-episode-003.json
    arc1-episode-004.json
    arc1-episode-005.json
    arc1-episode-006.json
    arc1-episode-007.json
    arc1-episode-008.json
    arc1-episode-009.json
    arc2-episode-001.json
    arc2-episode-002.json
    arc2-episode-003.json
    arc2-episode-004.json
    arc2-episode-005.json
    arc2-episode-006.json
    arc3-episode-001.json
    arc3-episode-002.json
    arc3-episode-003.json
    arc3-episode-004.json
    arc3-episode-005.json
    arc3-episode-006.json
    arc3-episode-007.json
    arc3-episode-008.json
    arc3-episode-009.json
  /cast/
    cast.json
Metadata Fields
Show Level (data/show/metashow.json)

showTitle: The official name of the audio drama series
logline: Short one-sentence description of the show's premise
synopsis: Extended description of the show's themes and narrative approach
extendedDescription: Longer, detailed description
showArtUrl: URL to the show cover art image 
networkDistributor: Platform hosting the show (e.g., Blubrry)
genreTags: Comma-separated genre and content tags (audio drama, sci-fi, horror, experimental)
imdbUrl: Link to the show's IMDb page
releaseDate: Show premiere date
showrunner: Name of creator/showrunner
showrunnerIsni: ISNI identifier for the showrunner (International Standard Name Identifier)
showrunnerPatreon: URL to showrunner's Patreon page
distributionLinks: Object containing platform-specific URLs

apple: Apple Podcasts URL
spotify: Spotify URL
blubrry: Blubrry hosting URL



Episode Level (data/episodes/*.json)

episodeId: Unique identifier for the episode (e.g., arc1-ep001)
title: Episode title
arc: Arc name (e.g., "Arc 1: The Chthonic")
episodeNumber: Formatted episode number (e.g., "Arc 1, Episode 1")
releaseDate: Publication date of the episode
logline: One-sentence summary of the episode
summary: Short description of the episode's plot and content
synopsis: Extended narrative summary
runtime: Episode duration (e.g., "45 minutes")
cast: Comma-separated list of voice actors in this episode
imdbUrl: Link to the episode's IMDb page (if available)
coverArtUrl: URL to episode-specific cover art (points to /images/episodes/ folder in GitHub)
distributionLinks: Object containing platform-specific episode URLs

apple: Apple Podcasts episode link
spotify: Spotify episode link
blubrry: Blubrry episode link
officialShowPage: URL on deepdreamstate.blubrry.net


showrunnerIsni: ISNI identifier for the creator
showrunnerPatreon: URL to creator's Patreon
distributor: Platform hosting (e.g., Blubrry)

Cast Level (data/cast/cast.json)
Array of cast and crew members, each containing:

name: Actor or crew member's name
role: Role type (e.g., "voice actor", "director", "producer")
imdbId: IMDb identifier (e.g., nm17760876)
charactersAndEpisodes: Comma-separated list of characters played and episodes they appear in

File Format
All metadata is stored as valid JSON for automated processing into JSON-LD schema markup and knowledge graph ingestion systems.
Image Assets
Images referenced in JSON files are hosted in the GitHub repository's /images/ folder:

/images/show/ - Show cover art
/images/episodes/ - Individual episode cover art

Image URLs in the JSON files point to the raw GitHub content URLs for direct access.
Knowledge Graph Integration
This metadata structure supports:

Schema.org markup: Converted to JSON-LD 
PodcastSeries/CreativeWork classification: Proper entity typing 
Linked data relationships: Episode-to-show, cast-to-episode, creator attribution
Cross-referencing: Authority linking for discoverability

Usage
This repository serves as the authoritative source for Deep Dream State metadata. 
