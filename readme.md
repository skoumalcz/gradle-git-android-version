## ✨ automagic! ✨

Append this to the bottom of your **root** `build.gradle`:

```groovy
apply from: "https://raw.githubusercontent.com/diareuse/gradle-git-android-version/semantic/android-version.gradle"
```

It will automatically set your versions according to rules of semantic versioning. It searches for 
 tag pattern `variant/*.*.*` where variant can be anything, anything before the slash is disregarded 
 in order to keep the same versions across all variants. 

As a matter of fact I've already made tagging utility [`taggy`](https://gist.github.com/diareuse/45d36f8755a0138cf339af160b4085f2) 
 which works for both `semantic` and `integration` styles. Unfortunately this tool works only on 
 linux-based systems.