# MathWorlds, Inc.

## Mission

Develop mathematics curriculum for children;
design and develop educational computer games and related online materials.

```
./gradlew generateSite
./gradlew serveSite
```

`generateSite` writes `_site` (GitHub Pages). Plugin id `org.podval.tools.site-publisher`.
A local site-publisher checkout at `../../Podval/site-publisher` is used when present
(`pluginManagement { includeBuild }` plus settings-body `includeBuild`, `-PsitePublisherDir=`);
CI resolves the plugin and `org.podval.tools:org.podval.tools.publisher` from Maven Central.

Do not push until a publisher with `asset: true` is on Maven Central (homepage
`index.yml`); then pin the plugin version if needed and push.
