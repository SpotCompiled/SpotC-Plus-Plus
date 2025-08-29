# SpotC++
<h1 align="center">

![GitHub all releases](https://img.shields.io/github/downloads/SpotCompiled/SpotC-Plus-Plus/total?label=Downloads&style=for-the-badge) 
![GitHub Repo stars](https://img.shields.io/github/stars/SpotCompiled/SpotC-Plus-Plus?label=Stars&style=for-the-badge) 
![GitHub release (latest by date)](https://img.shields.io/github/v/release/SpotCompiled/SpotC-Plus-Plus?label=Release&style=for-the-badge) 
![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/SpotCompiled/SpotC-Plus-Plus?include_prereleases&label=PRE-Release&style=for-the-badge) 

</h1>

<br/>This is my repo for compiled EeveeSpotify + Sposify IPAs. EeveeSpotify is a Spotify IOS app tweak that removes ads, removes limited skips, and almost every other premium feature. The only main premium feature that does not work is offline downloads, as this is done server-side. Sposify is a Spotify IOS app tweak that adds various enhancements to the Spotify IOS application.

***

## Installing

<details>
<summary><h3>Adding to AltStore/SideStore</h3></summary>

### Option One:<br/>
You can add my repo to AltStore or SideStore for automatic updates and conviniance, by following the steps below:<br/>
[Click this link](https://spotc-repo.yodaluca.dev/AltStoreAdd) on your device with SideStore/AltStore and it will open SideStore/AltStore with it prompting you to add the source.

### Option Two:<br/>
You can add my repo to AltStore *Beta* or SideStore for automatic updates and conviniance, by following the steps below:<br/>
1. Tap "Sources" in the top-right corner of the Browse tab.<br/>
2. Tap the ”+” button and add my source by entering its URL "[https://spotc-repo.yodaluca.dev/AltStore%20Repo.json](https://spotc-repo.yodaluca.dev/AltStore%20Repo.json)"
3. Now any "SpotC" Apps will show up in AltStore/SideStore under the "Browse" tab where you can install and update my apps easily from within AltStore/SideStore.

</details>

<details>
<summary><h3>Adding to Scarlet/Others</h3></summary>

You can add my repo to Scarlet and other sideloading apps for automatic updates and conviniance, by following the steps below:<br/>
1. Press and hold the Install button in top right.
2. Select "Add Repo"
3. Enter the URL "[https://spotc-repo.yodaluca.dev/Scarlet%20Repo.json](https://spotc-repo.yodaluca.dev/Scarlet%20Repo.json)"
4. Now any "SpotC" Apps will show up in Scarlet (or other sideloading apps) where you can install and update my apps easily from within Scarlet.<br/>

</details>

You can also download from [the website](https://spotc.yodaluca.dev) and use with whatever app/service you wish.

***

## How do I add my "Musixmatch token"?<br/>
In version 2.2.0 the option to use Musixmatch as a lyric provider was added, you must add your user token so that the app may access the Musixmatch API. However, in version 2.3.4 you can now request an anonymous Musixmatch token, simply by pressing the button when prompted for a token, if you want to use your own you can follow the following instructions below.
<details>
<summary>Intructions</summary><be>
1. Download the Musixmatch Lyrics Finder app from the app store.<br/>
2. Open the Musixmatch app.<br/>
3. Login/Create an account.<br/>
4. Go to settings (Top right corner) > Scroll all the way down > click "Get help" > click "Copy debug info"<br/>
5. Paste this into SpotC++, when it asks you for your user token.<br/>
</details>

## How it's Made<br/>
I post a new release every time there is an EeveeSpotify/Sposify Update, or there is a new major Spotify update that is compatible with both the latest EeveeSpotify and the latest Sposify. I get the vanilla Spotify IPA from IOS God's [Decrypted AppStore](https://armconverter.com/decryptedappstore/us/spotify), from green verified links on [AppDB](https://appdb.to/app/ios/324684580), or using [BagBak](https://github.com/ChiChou/bagbak), with my personal jailbroken iPhone XR. I will specify details on each release page. Then I download the latest EeveeSpotify .deb and SwiftProtobuf framework .deb (dependency) from Eevee's release page [here](https://github.com/whoeevee/EeveeSpotify/releases/latest) and Orion Runtime (iOS 14 - 16) off of Chariz [here](https://chariz.com/get/orion-runtime14) (it's a dependency). I also download the latest commit of Eevee's [OpenSpotifySafariExtension](https://github.com/whoeevee/OpenSpotifySafariExtension). As well as the latest Sposify .deb from  Dynastic repo [here](https://repo.dynastic.co/package/com.spos). Sposify has bugs that are patched by [SposifyFix](https://level3tjg.me/repo) by level3tjg, I download this aswell. I download the tweaks directly from the sources. I then inject the .deb's and .appx into the Spotify IPA using [my fork](https://github.com/SpotCompiled/pyzule-rw) of [Cyan](https://github.com/asdfzxcvbn/pyzule-rw), and change the IPA version and Bundle ID to the SpotC++ version and Bundle ID. (For the AltStore Version) I do not do anything else to the IPA (Unless otherwise specified in the release notes)... All of this and more is automated using the completely open-source GitHub Workflow script available [here](https://github.com/SpotCompiled/SpotC-Plus-Plus/blob/main/.github/workflows/Build%20and%20Release.yml).

Version Format is *SpotC++ Version*\_*Spotify Version*<br/>
Ex. *v1.3.6*\_*v8.7.78*<br/>

## Credits:<br/>
[IOS God's Decrypted App Store](https://armconverter.com/decryptedappstore/us/spotify) and [AppDB](https://appdb.to/app/ios/324684580)- *Decrypted Vanilla Spotify IPA*<br/>
[julioverne-  Spotilife](https://julio.hackyouriphone.org/) *For the original Spotilife tweak*<br/>
[aesthyrica- Sposify](https://repo.dynastic.co/package/com.spos) *For Sposify tweaked  .deb*<br/>
[Whoeevee-  EeveeSpotify](https://github.com/whoeevee/EeveeSpotify) *For EeveeSpotify tweaked .deb*<br/>
[ChiChou & Asdfzxcvbn-  BagBak](https://github.com/ChiChou/bagbak) *For BagBak used to decrypt .ipa*<br/>
[Asdfzxcvbn-  Cyan](https://github.com/asdfzxcvbn/pyzule-rw) *Used to inject tweaks and modify the .ipa*<br/>
[Theos Team-  Orion Runtime (iOS 14 - 16)](https://chariz.com/get/orion-runtime14) *For Orion Runtime (iOS 14 - 16) tweaked .deb*<br/>
[Apple inc.-  Swift Protobuf](https://github.com/apple/swift-protobuf)<br/>
[level3tjg- Sposify Fix](https://level3tjg.me/repo/) *For Sposify Fix tweaked  .deb*<br/>
[Am1nCmd- Spotify++](https://appdb.to/app/cydia/1900000540) *For ScreenShots*<br/>
[@RobyRew](https://github.com/RobyRew) *For helping me setup a lot of things*
***
<sup>We are not affiliated, associated, authorized, endorsed by, or in any way officially connected with any other company, agency, or government agency. All product and company names are trademarks™ or registered® trademarks of their respective holders. Use of them does not imply any affiliation with or endorsement by them.

<sup>The software is provided "as is," without any warranties, whether express or implied, including but not limited to warranties of merchantability or fitness for a particular purpose. The developers make no guarantees regarding the software’s performance, reliability, or accuracy. In no event shall the developers be held liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or its use. Use of this software is at your own risk.

<sup>Furthermore, the software may utilize or depend on third-party software, libraries, or services. The developers are not liable for any issues, errors, or damages resulting from the use of such third-party components. The providers of those components are likewise not responsible for any liabilities arising from their use in this software.

<sup>By using this software, you acknowledge and accept full responsibility for any risks associated with its use.
