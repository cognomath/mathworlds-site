# MathWorlds, Inc.

## Mission

Develop mathematics curriculum for children;
design and develop educational computer games and related online materials.

```
./gradlew generateSite
./gradlew serveSite
```

`generateSite` writes `_site` (GitHub Pages). A local site-publisher checkout at
`../../Podval/site-publisher` is used when present (`-PsitePublisherDir=`); CI
resolves `org.podval.tools:org.podval.tools.publisher` from Maven Central.
