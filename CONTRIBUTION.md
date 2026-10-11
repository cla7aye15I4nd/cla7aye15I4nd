# Open-source contributions

My contributions across merged upstream code, vulnerability reports, and patch validation. Work submitted through [cla7aye15I4nd](https://github.com/cla7aye15I4nd) and my alternate account [oss-patch](https://github.com/oss-patch) is included here.

Some fixes were assisted by [PatchAgent](https://github.com/cla7aye15I4nd/PatchAgent); those records are identified below. Each project appears once, with links to the original evidence.

Last reviewed: **2026-10-11**. This is a record of the public contributions located so far; older identities and other hosting platforms may contain additional history.

[Back to profile](README.md)

## Projects

| Project | Contribution records |
| --- | --- |
| [ANGLE](#angle) | commits, reports / credits / reviews |
| [angr](#angr) | bug reports |
| [Assimp](#assimp) | commits, pull requests, bug reports |
| [Augeas](#augeas) | bug reports |
| [BlueZ](#bluez) | bug reports |
| [C-Blosc2](#c-blosc2) | bug reports |
| [CTF Wiki](#ctf-wiki) | commits, pull requests |
| [curl](#curl) | commits |
| [FFmpeg](#ffmpeg) | commits |
| [free5GC gtp5g](#free5gc-gtp5g) | commits, pull requests |
| [GitProxy](#gitproxy) | commits, reports / credits / reviews |
| [GNU Aspell](#gnu-aspell) | bug reports |
| [GPAC](#gpac) | commits, pull requests |
| [GPTFuzz](#gptfuzz) | commits, pull requests |
| [HDF5](#hdf5) | commits, pull requests |
| [jq](#jq) | commits, bug reports |
| [LibreDWG](#libredwg) | commits, pull requests |
| [libssh2](#libssh2) | commits, pull requests |
| [LibTIFF](#libtiff) | commits |
| [Linux](#linux) | commits |
| [mJS](#mjs) | bug reports |
| [Nokogiri](#nokogiri) | reports / credits / reviews |
| [ntopng](#ntopng) | bug reports |
| [Oj](#oj) | reports / credits / reviews |
| [open62541](#open62541) | commits, bug reports |
| [OpenWrt LuCI](#openwrt-luci) | reports / credits / reviews |
| [PcapPlusPlus](#pcapplusplus) | commits, pull requests |
| [PCL](#pcl) | commits, bug reports |
| [PHP](#php) | commits, pull requests, bug reports |
| [Python](#python) | commits, pull requests |
| [Qiling](#qiling) | commits, pull requests |
| [Sentry](#sentry) | commits, pull requests |
| [ShivyC](#shivyc) | commits, pull requests |
| [sqlite3-ruby](#sqlite3-ruby) | commits, reports / credits / reviews |
| [TileLang](#tilelang) | commits, pull requests |
| [Unicorn](#unicorn) | commits, bug reports |
| [Wasm3](#wasm3) | commits, pull requests |
| [Wasmtime](#wasmtime) | commits, bug reports |
| [Yasm](#yasm) | commits, pull requests |
| [PintOS](#pintos) | commits, pull requests |

Only merged upstream code is listed here. Unmerged pull requests, fork-only development, and general discussion are excluded. Reporting and patch-validation credits are labeled separately from code authorship.

## Contribution records

### ANGLE

[Project repository](https://github.com/google/angle)

- Reported the `TIntermCase` null-pointer issue in June 2026; the maintainer fix was merged on June 26. [Public review #8007986](https://chromium-review.googlesource.com/c/angle/angle/+/8007986).

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`6e65aeaa70`](https://chromium.googlesource.com/angle/angle/+/6e65aeaa70062023f988c569075e5b1b6d41943c) | \[translator\] Fix cloning switch case nodes without a condition | Reported issue; fix authored by maintainer |

</details>

### angr

[Project repository](https://github.com/angr/angr)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Bug in block.pp()](https://github.com/angr/angr/issues/3140) — Maintainer confirmed fixed in current angr versions. Evidence: [maintainer response](https://github.com/angr/angr/issues/3140#issuecomment-5374934981).

</details>

### Assimp

[Project repository](https://github.com/assimp/assimp)

<details>
<summary>Pull requests (3)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Fix invalid access](https://github.com/assimp/assimp/pull/5765) | Merged | Upstream: `assimp/assimp` | cla7aye15I4nd · PatchAgent-assisted |
| [Fix stack overflow](https://github.com/assimp/assimp/pull/5764) | Merged | Upstream: `assimp/assimp` | cla7aye15I4nd · PatchAgent-assisted |
| [Fix buffer overflow in MD3Loader](https://github.com/assimp/assimp/pull/5763) | Merged | Upstream: `assimp/assimp` | cla7aye15I4nd · PatchAgent-assisted |

</details>

<details>
<summary>Bug and vulnerability reports (7)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Bug: Heap-based Buffer Overflow in `SkipSpacesAndLineEnd`](https://github.com/assimp/assimp/issues/5860) — Fixed by an upstream merged PR. Evidence: [fix PR](https://github.com/assimp/assimp/pull/5921), [fix commit](https://github.com/assimp/assimp/commit/ecc8a1c8695560df108d6adc00b3d7b1ba15df9f).
- [Bug: NULL Pointer Dereference in `Assimp::SplitLargeMeshesProcess_Triangle::UpdateNode`](https://github.com/assimp/assimp/issues/5791) — Fixed by an upstream merged PR. Evidence: [fix PR](https://github.com/assimp/assimp/pull/5799), [fix commit](https://github.com/assimp/assimp/commit/ecdf8d24b85367b22ba353b4f82299d4af7f1f97).
- [Bug:Use After Free in the `CallbackToLogRedirector `](https://github.com/assimp/assimp/issues/5790) — Report submitted; no specific accepted fix verified yet.
- [Bug:SEGV in `SortByPTypeProcess::Execute`](https://github.com/assimp/assimp/issues/5789) — Maintainer tracking in epic #6128; remains open. Evidence: [maintainer response](https://github.com/assimp/assimp/issues/5789#issuecomment-2845738979).
- [Bug:Use After Free in the `CallbackToLogRedirector `](https://github.com/assimp/assimp/issues/5788) — Fixed by an upstream merged PR. Evidence: [fix PR](https://github.com/assimp/assimp/pull/5918), [fix commit](https://github.com/assimp/assimp/commit/f12e52198669239af525e525ebb68407977f8e34).
- [Bug: Heap-based Buffer Overflow in OpenDDLParser::parseStructure](https://github.com/assimp/assimp/issues/5787) — Fixed by an upstream merged PR. Evidence: [fix PR](https://github.com/assimp/assimp/pull/5919), [fix commit](https://github.com/assimp/assimp/commit/2b773f0f5a726c38dda72307b5311c14fc3a76ae), [maintainer response](https://github.com/assimp/assimp/issues/5787#issuecomment-2546889997).
- [Bug: Heap Buffer Overflow in the `MD5Importer::LoadMD5MeshFile`](https://github.com/assimp/assimp/issues/5771) — Maintainer tracking in epic #6128; remains open. Evidence: [maintainer response](https://github.com/assimp/assimp/issues/5771#issuecomment-2840005711), [maintainer response](https://github.com/assimp/assimp/issues/5771#issuecomment-2845697408).

</details>

<details>
<summary>Commits and patchsets (7)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`ab12e8d8ba`](https://github.com/assimp/assimp/commit/ab12e8d8baecac95daa23ebb5528fe3d90e3c71e) | Fix stack overflow (#5764) | Authored commit |
| [`3bd98611d7`](https://github.com/assimp/assimp/commit/3bd98611d70e973b4f62cccc8e17519984d07588) | Fix buffer overflow in MD3Loader (#5763) | Authored commit |
| [`d468e633b1`](https://github.com/assimp/assimp/commit/d468e633b1b5cf20b893ef0315006fa6b901ca8d) | Fix invalid access (#5765) | Authored commit |
| [`ecc8a1c869`](https://github.com/assimp/assimp/commit/ecc8a1c8695560df108d6adc00b3d7b1ba15df9f) | Fix buffer overflow in MD5Parser::SkipSpacesAndLineEnd | Reported bug; maintainer-authored fix |
| [`ecdf8d24b8`](https://github.com/assimp/assimp/commit/ecdf8d24b85367b22ba353b4f82299d4af7f1f97) | SplitLargeMeshes: Fix crash | Reported bug; maintainer-authored fix |
| [`f12e521986`](https://github.com/assimp/assimp/commit/f12e52198669239af525e525ebb68407977f8e34) | Fix use after free in the CallbackToLogRedirector | Reported bug; maintainer-authored fix |
| [`2b773f0f5a`](https://github.com/assimp/assimp/commit/2b773f0f5a726c38dda72307b5311c14fc3a76ae) | Fix heap-buffer-overflow in OpenDDLParser | Reported bug; maintainer-authored fix |

</details>

### Augeas

[Project repository](https://github.com/hercules-team/augeas)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Segmentation Fault in Augeas 1.14.1 When Evaluating Expressions](https://github.com/hercules-team/augeas/issues/848) — Report submitted; no specific accepted fix verified yet.

</details>

### BlueZ

[Project repository](https://github.com/bluez/bluez)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Heap Buffer Overflow in fuzz_xml for BlueZ Commit 9d69dba](https://github.com/bluez/bluez/issues/1005) — Closed as stale / not planned; no maintainer acceptance or fix verified.

</details>

### C-Blosc2

[Project repository](https://github.com/Blosc/c-blosc2)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Heap-buffer-overflow in decompress_frame_fuzzer (oss-fuzz build)](https://github.com/Blosc/c-blosc2/issues/639) — Maintainer acknowledged the report and invited a fix PR; no merged fix verified. Evidence: [maintainer response](https://github.com/Blosc/c-blosc2/issues/639#issuecomment-2458955114).

</details>

### CTF Wiki

[Project repository](https://github.com/ctf-wiki/ctf-wiki)

<details>
<summary>Pull requests (5)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Update cbc.md](https://github.com/ctf-wiki/ctf-wiki/pull/557) | Merged | Upstream: `ctf-wiki/ctf-wiki` | cla7aye15I4nd |
| [Update cbc-zh.md](https://github.com/ctf-wiki/ctf-wiki/pull/556) | Merged | Upstream: `ctf-wiki/ctf-wiki` | cla7aye15I4nd |
| [add a md5 tool](https://github.com/ctf-wiki/ctf-wiki/pull/525) | Merged | Upstream: `ctf-wiki/ctf-wiki` | cla7aye15I4nd |
| [添加CBC字节反转攻击的介绍和例子](https://github.com/ctf-wiki/ctf-wiki/pull/520) | Merged | Upstream: `ctf-wiki/ctf-wiki` | cla7aye15I4nd |
| [Update rsa_e_attack.md](https://github.com/ctf-wiki/ctf-wiki/pull/313) | Merged | Upstream: `ctf-wiki/ctf-wiki` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (5)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`6ea2d63718`](https://github.com/ctf-wiki/ctf-wiki/commit/6ea2d63718559c8e21e2813aff79012cb19d44b4) | Update cbc.md | Authored commit |
| [`0d360139ec`](https://github.com/ctf-wiki/ctf-wiki/commit/0d360139ec97b3e977092fb4415c80ee9935470b) | Update cbc-zh.md | Authored commit |
| [`3ceee42a43`](https://github.com/ctf-wiki/ctf-wiki/commit/3ceee42a43e231d49e6588d272aee8551b4649a1) | Update md5.md | Authored commit |
| [`67c0d3f6a3`](https://github.com/ctf-wiki/ctf-wiki/commit/67c0d3f6a391fe91c200625815866ba310ceb2c1) | 添加CBC字节反转攻击的介绍和例子 | Authored commit |
| [`0f27ff5b4d`](https://github.com/ctf-wiki/ctf-wiki/commit/0f27ff5b4dea1264afeca25b760f397845c4e0d6) | Update rsa_e_attack.md | Authored commit |

</details>

### curl

[Project repository](https://github.com/curl/curl)

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`10bf036282`](https://github.com/curl/curl/commit/10bf0362826681dd745b8eb06dee2af23a6a317c) | share link: forget connection | Authored commit |

</details>

### FFmpeg

[Project repository](https://github.com/FFmpeg/FFmpeg)

<details>
<summary>Commits and patchsets (32)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`87941e8765`](https://github.com/FFmpeg/FFmpeg/commit/87941e8765c129bd9f3090481145772f14d14fb8) | avfilter/vf_tiltandshift: keep the initial black padding within the frame | Finding / reporting credit |
| [`f391d256fd`](https://github.com/FFmpeg/FFmpeg/commit/f391d256fdeb64245f2693e85ebd662e09262124) | avcodec/dcaenc: fill the LFE history from the LFE channel | Finding / reporting credit |
| [`9e1918b513`](https://github.com/FFmpeg/FFmpeg/commit/9e1918b513fef04cd656f68fa0f611561456badc) | avfilter/vf_ssim360: use the sample stride for the tape maps | Finding / reporting credit |
| [`6ae78e8554`](https://github.com/FFmpeg/FFmpeg/commit/6ae78e85548238b5887331e8f000a701a58fa125) | avformat/tee_common: reject slave options without a closing bracket | Finding / reporting credit |
| [`9edd06f861`](https://github.com/FFmpeg/FFmpeg/commit/9edd06f8612c242b83bf9e3d14aa85180015a211) | avcodec/proresenc_kostya: fill macroblock rows past the end of the bottom field | Finding / reporting credit |
| [`d74f5e0559`](https://github.com/FFmpeg/FFmpeg/commit/d74f5e0559ba09d942c47687856349b03c1115dd) | avcodec/proresenc_anatoliy: fill the slice from the field's own number of lines | Finding / reporting credit |
| [`ed27b2c498`](https://github.com/FFmpeg/FFmpeg/commit/ed27b2c498e343cd68f2871da535c2a37525087b) | avcodec/mjpegenc: flip AMV pictures starting from the last row of each plane | Finding / reporting credit |
| [`6cf8bfb57d`](https://github.com/FFmpeg/FFmpeg/commit/6cf8bfb57dece3f932d5275be8e810de6042838b) | avformat/rtpenc_latm: check that the PayloadLengthInfo fits the RTP payload | Finding / reporting credit |
| [`97840ddfbb`](https://github.com/FFmpeg/FFmpeg/commit/97840ddfbbed2750788e7965f4961d7dbe6a4f5f) | avcodec/ratecontrol: reject picture types other than I, P and B in the pass 2 statistics | Finding / reporting credit |
| [`da555d4caa`](https://github.com/FFmpeg/FFmpeg/commit/da555d4caaa2b9a71eef85a46b1ec727286a8be8) | avcodec/diracdec: fail on a data unit whose size does not fit the bit reader | Finding / reporting credit |
| [`733bec3e19`](https://github.com/FFmpeg/FFmpeg/commit/733bec3e19759520ccdbeb6c3c0cae280bbe6dc5) | avcodec/nellymoserenc: keep the trellis index below OPT_SIZE | Finding / reporting credit |
| [`1088e8b43e`](https://github.com/FFmpeg/FFmpeg/commit/1088e8b43e7f367a7311b7a51410fcf149d6cda8) | avformat/asfdec_f: index the seek position table by ASF stream number | Finding / reporting credit |
| [`b8b8d43935`](https://github.com/FFmpeg/FFmpeg/commit/b8b8d4393548b9bd1cbbced220131b81e268a821) | avcodec/h274: free the big endian pixel buffer before the context that holds it | Finding / reporting credit |
| [`8864fd0aec`](https://github.com/FFmpeg/FFmpeg/commit/8864fd0aecf21fe9e3cfcd83a8ef33cb7e885fd4) | avcodec/cbs_h265: bound the number of decoding units by the picture size and the slice segment limit | Finding / reporting credit |
| [`3e09f5e24e`](https://github.com/FFmpeg/FFmpeg/commit/3e09f5e24eb277a6d011745ff03e602f61c5c171) | avcodec/cook: require the channel mask to cover every subpacket channel | Finding / reporting credit |
| [`8702f12c9d`](https://github.com/FFmpeg/FFmpeg/commit/8702f12c9daa199cc4d7c17164b13c3cdcdc2436) | avcodec/dvdsubenc: account for the byte alignment of each RLE line | Finding / reporting credit |
| [`f8c4c6400e`](https://github.com/FFmpeg/FFmpeg/commit/f8c4c6400e835bf65e8b9cc12aba9e5c4d1c818c) | avcodec/hap: do not hide the failure of the chunk table allocation | Finding / reporting credit |
| [`c9581b4eb8`](https://github.com/FFmpeg/FFmpeg/commit/c9581b4eb842dddd77f23b88416ef678986b5099) | fftools/ffprobe: name the film grain components and pieces | Finding / reporting credit |
| [`4800bf20d8`](https://github.com/FFmpeg/FFmpeg/commit/4800bf20d82243fb8e3131061d3a3e70536c42fa) | avcodec/cfhd: check the channel number after every tag | Finding / reporting credit |
| [`2731412616`](https://github.com/FFmpeg/FFmpeg/commit/273141261699b660eed1b1c070fb8b1dd88c5218) | avcodec/nellymoserenc: initialize the trellis table row by row | Finding / reporting credit |
| [`8e55f4f3e9`](https://github.com/FFmpeg/FFmpeg/commit/8e55f4f3e9eb05073b2738e7a3d99670777e5e04) | avcodec/v210dec: reject a custom_stride smaller than one row | Finding / reporting credit |
| [`912208af28`](https://github.com/FFmpeg/FFmpeg/commit/912208af28f8762e8d59263639c4728a2a3c087a) | avcodec/dcadec: ignore reserved speaker positions in coded channel order | Finding / reporting credit |
| [`bfac54a03b`](https://github.com/FFmpeg/FFmpeg/commit/bfac54a03b9c1046d8956b9674bb21167e230eb9) | avformat/hlsenc: reject hls_enc_key and hls_enc_iv values shorter than 16 bytes | Finding / reporting credit |
| [`abad70c575`](https://github.com/FFmpeg/FFmpeg/commit/abad70c57548cc8089d81a1126f02b20f3e95e8e) | fftools/ffprobe: refuse the diagram output formats | Finding / reporting credit |
| [`971ea9d6a2`](https://github.com/FFmpeg/FFmpeg/commit/971ea9d6a2a9ae4c770936f0569cf40720d4c304) | avcodec/dovi_rpuenc: compress the DM metadata only against previous DM metadata | Finding / reporting credit |
| [`5408059eb7`](https://github.com/FFmpeg/FFmpeg/commit/5408059eb7f2ff628ba25db7ff8714e707467c49) | avformat/cafdec: fix negative index use in read_seek | Patch validation credit |
| [`52b78cd3fe`](https://github.com/FFmpeg/FFmpeg/commit/52b78cd3fe411662b1db06e63c17b5d1399155ee) | avformat/rtmpproto: validate compressed SWF header length | Patch validation credit |
| [`f1c3f1cae1`](https://github.com/FFmpeg/FFmpeg/commit/f1c3f1cae1bbe51d61fea461954b70882c3800ff) | avformat/avidec: validate INFO list size before parsing | Patch validation credit |
| [`8010aa2193`](https://github.com/FFmpeg/FFmpeg/commit/8010aa2193f5a354394a36eb7bfb57deaaf81c2e) | avformat/rtpdec_mpeg4: reject zero-length AU header sections | Patch validation credit |
| [`25a98586cc`](https://github.com/FFmpeg/FFmpeg/commit/25a98586cc651bcf0419fcb2453b51ffa8f2fb86) | fftools/ffmpeg_opt: validate stream index in negative map handling | Patch validation credit |
| [`1a00ea51cb`](https://github.com/FFmpeg/FFmpeg/commit/1a00ea51cbaf3967718ee0ceeb51a127d42bd249) | avformat/rtsp: Fix out-of-bounds read in SDP parser when control_url is empty | Patch validation credit |
| [`664d44a825`](https://github.com/FFmpeg/FFmpeg/commit/664d44a8254813a6d78432e57e02223a1e185467) | avformat/rtpdec_latm: avoid integer overflow in LATM length parsing | Patch validation credit |

</details>

### free5GC gtp5g

[Project repository](https://github.com/free5gc/gtp5g)

<details>
<summary>Pull requests (1)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Fix IFLA_GTP5G_PDR_HASHSIZE divide error](https://github.com/free5gc/gtp5g/pull/166) | Merged | Upstream: `free5gc/gtp5g` | oss-patch · PatchAgent-assisted |

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`3acfd60b96`](https://github.com/free5gc/gtp5g/commit/3acfd60b96c72dbb25e105c4dc00f116156e1039) | Fix IFLA_GTP5G_PDR_HASHSIZE divide error (#166) | Authored commit; PatchAgent-assisted |

</details>

### GitProxy

[Project repository](https://github.com/finos/git-proxy)

- [GHSA-293g-m6p5-4fqq](https://github.com/finos/git-proxy/security/advisories/GHSA-293g-m6p5-4fqq) — Arbitrary directory deletion via path traversal in the push id. Official finder credit. Fixed in 2.0.2, 2.1.2.
- [GHSA-w285-c89q-mg53](https://github.com/finos/git-proxy/security/advisories/GHSA-w285-c89q-mg53) — git-receive-pack PACK parsing can exhaust process resources. Official reporter credit. Fixed in 2.0.2, 2.1.2.
- [v2.2.0 release notes](https://github.com/finos/git-proxy/releases/tag/v2.2.0) thank my account for finding and reporting these issues. The PACK fix explicitly credits the patch I supplied.

<details>
<summary>Commits and patchsets (2)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`2ae671ac02`](https://github.com/finos/git-proxy/commit/2ae671ac022bb9fd7e7a7c742c6fb48d7e68820c) | Validate object IDs and confine checkout directories | Finding credit; maintainer-authored fix |
| [`4e8859f3b2`](https://github.com/finos/git-proxy/commit/4e8859f3b23000c3e82d080c351926fd793731a5) | Bound PACK decompression and packet parsing | Reported issue and supplied patch; integrated by maintainer |

</details>

### GNU Aspell

[Project repository](https://github.com/GNUAspell/aspell)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Assertion Failure in acommon::ObjStack::check_size in aspell_fuzzer](https://github.com/GNUAspell/aspell/issues/657) — Report submitted; no specific accepted fix verified yet.

</details>

### GPAC

[Project repository](https://github.com/gpac/gpac)

<details>
<summary>Pull requests (1)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Remove duplicate checks](https://github.com/gpac/gpac/pull/2696) | Merged | Upstream: `gpac/gpac` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`344811bd8d`](https://github.com/gpac/gpac/commit/344811bd8d768d53e27c8aa99492e7c884835154) | Remove duplicate checks | Authored commit |

</details>

### GPTFuzz

[Project repository](https://github.com/hubertyoo/GPTFuzz)

<details>
<summary>Pull requests (2)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Fix some bugs](https://github.com/hubertyoo/GPTFuzz/pull/11) | Merged | Upstream: `hubertyoo/GPTFuzz` | cla7aye15I4nd |
| [Add log function](https://github.com/hubertyoo/GPTFuzz/pull/10) | Merged | Upstream: `hubertyoo/GPTFuzz` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (33)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`e3547757d5`](https://github.com/hubertyoo/GPTFuzz/commit/e3547757d593793b5e181274561f275c1623b67e) | Fix some typos | Authored commit |
| [`c4ca8a9723`](https://github.com/hubertyoo/GPTFuzz/commit/c4ca8a97230cdb41d029374354f8d37a8923b09b) | Revert "Merge branch 'master' into next" | Authored commit |
| [`4fc4540f68`](https://github.com/hubertyoo/GPTFuzz/commit/4fc4540f6828ae69c0db49c4391b94918548abb4) | Merge branch 'master' into next | Authored commit |
| [`bff8e81450`](https://github.com/hubertyoo/GPTFuzz/commit/bff8e8145096f10a9000b0b43560add129067157) | format some code and remove some comment | Authored commit |
| [`c9588b8368`](https://github.com/hubertyoo/GPTFuzz/commit/c9588b8368133073e8deec2d117af85aad179832) | Update core.py | Authored commit |
| [`bd927cdb66`](https://github.com/hubertyoo/GPTFuzz/commit/bd927cdb66ed619c96b37051e16e86d121686c18) | fix some typos | Authored commit |
| [`22e52c44d8`](https://github.com/hubertyoo/GPTFuzz/commit/22e52c44d8f0a0d081be6c119d9d707f07d5acce) | fix some arguments error | Authored commit |
| [`a91d059bb5`](https://github.com/hubertyoo/GPTFuzz/commit/a91d059bb5f9d156c8d919a8e6e9a45ac4c7b35c) | Add logger | Authored commit |
| [`fad027abba`](https://github.com/hubertyoo/GPTFuzz/commit/fad027abbafa7e2c2c9605fd37ead6693e0e3ae3) | Update some api interface | Authored commit |
| [`102b342231`](https://github.com/hubertyoo/GPTFuzz/commit/102b342231673684d9da5875f2ded560c6747317) | Fix a typo | Authored commit |
| [`77861de0b0`](https://github.com/hubertyoo/GPTFuzz/commit/77861de0b0f986572784039d3f723dc14e45d1fd) | Remove redundant code | Authored commit |
| [`7bb8c6adb9`](https://github.com/hubertyoo/GPTFuzz/commit/7bb8c6adb90e2bf3715e393594342e2219acc572) | Update the mutator | Authored commit |
| [`519e4c9238`](https://github.com/hubertyoo/GPTFuzz/commit/519e4c9238f9291a1708283a078e3866f700330a) | Fix a typo | Authored commit |
| [`4ea43aa2ca`](https://github.com/hubertyoo/GPTFuzz/commit/4ea43aa2ca4e4450d4f193c9389180277d1d1c79) | Update openai key interface | Authored commit |
| [`c2aaf06ce9`](https://github.com/hubertyoo/GPTFuzz/commit/c2aaf06ce9c1af9a10ad5c033b35bd369dcb1744) | Add a example | Authored commit |
| [`4233ce654d`](https://github.com/hubertyoo/GPTFuzz/commit/4233ce654dfda1d5b782b0baef8510ea59e4b85e) | Refactor some type anotation | Authored commit |
| [`b21c4024df`](https://github.com/hubertyoo/GPTFuzz/commit/b21c4024dfad2fd0ba7af94c7a4f02cba32f98a0) | Fix class name | Authored commit |
| [`95f27c28ef`](https://github.com/hubertyoo/GPTFuzz/commit/95f27c28eff3fcb6423d6450d0d61cda86f8b4e2) | Remove files have refactored | Authored commit |
| [`564b1d72b4`](https://github.com/hubertyoo/GPTFuzz/commit/564b1d72b4dae1298f3a4010ad8c6c1ec924df46) | Update README.md | Authored commit |
| [`c0d5a9b891`](https://github.com/hubertyoo/GPTFuzz/commit/c0d5a9b8914fd7431c226a84c1336c031aa04218) | Add 3 selection policy | Authored commit |
| [`3bb61eadd9`](https://github.com/hubertyoo/GPTFuzz/commit/3bb61eadd9bf40d540ee60aa5ca4c2d2472429aa) | Add predictor | Authored commit |
| [`cb4da350b7`](https://github.com/hubertyoo/GPTFuzz/commit/cb4da350b751588561786b1f2e6fa08a6b8523b3) | Almost finish the entire framework | Authored commit |
| [`e1a86ea06d`](https://github.com/hubertyoo/GPTFuzz/commit/e1a86ea06d56de1b584a91b893fccd008f56aa59) | Remove magic string | Authored commit |
| [`1d43e7e081`](https://github.com/hubertyoo/GPTFuzz/commit/1d43e7e08125321798411094213a55080a66375e) | Fix class name | Authored commit |
| [`a568ca7256`](https://github.com/hubertyoo/GPTFuzz/commit/a568ca7256b0ef3d165df70585529ce0e95996d9) | Almost finish the basic framework | Authored commit |
| [`94d10cbff9`](https://github.com/hubertyoo/GPTFuzz/commit/94d10cbff9e8bfd29bb957ab7bb9187d2eee1f34) | Fix annotation | Authored commit |
| [`a50bb3ba87`](https://github.com/hubertyoo/GPTFuzz/commit/a50bb3ba87f5b20e7899ebcff654226cd12f9f84) | Add fuzzer framework | Authored commit |
| [`625c81b929`](https://github.com/hubertyoo/GPTFuzz/commit/625c81b929ef6c0962ff7cb1b08fb3f34b31eb14) | Fix the class name | Authored commit |
| [`db45ec6464`](https://github.com/hubertyoo/GPTFuzz/commit/db45ec6464dcb41135d7059c83e6aa0971e9e824) | Add utils module | Authored commit |
| [`12ab6a0cf9`](https://github.com/hubertyoo/GPTFuzz/commit/12ab6a0cf9cce5429186f1d54084cbe98e8da0c8) | Update mutator file format | Authored commit |
| [`8c676194b2`](https://github.com/hubertyoo/GPTFuzz/commit/8c676194b25919626cb072e5cac70dd055a99b5c) | Update Basic seed selection | Authored commit |
| [`35f94f37ca`](https://github.com/hubertyoo/GPTFuzz/commit/35f94f37ca9423fc70f065b4e9007572a39cc949) | Fix a typo in mutator | Authored commit |
| [`43b8d21a4b`](https://github.com/hubertyoo/GPTFuzz/commit/43b8d21a4b82a2e94c64b2b6d9d9353bc09d44c5) | Finish the mutator refactor | Authored commit |

</details>

### HDF5

[Project repository](https://github.com/HDFGroup/hdf5)

<details>
<summary>Pull requests (2)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Fix vuln OSV-2023-77](https://github.com/HDFGroup/hdf5/pull/5210) | Merged | Upstream: `HDFGroup/hdf5` | oss-patch · PatchAgent-assisted |
| [Fix vuln OSV-2024-390](https://github.com/HDFGroup/hdf5/pull/5201) | Merged | Upstream: `HDFGroup/hdf5` | oss-patch · PatchAgent-assisted |

</details>

<details>
<summary>Commits and patchsets (2)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`7f27ba8c3a`](https://github.com/HDFGroup/hdf5/commit/7f27ba8c3a8483c3d7e5e2cb21fefb2c7563422d) | Fix vuln OSV-2023-77 (#5210) | Authored commit; PatchAgent-assisted |
| [`c0192e2361`](https://github.com/HDFGroup/hdf5/commit/c0192e236122f483c71723d66dddee2cdc80ed5a) | Fix vuln OSV-2024-390 (#5201) | Authored commit; PatchAgent-assisted |

</details>

### jq

[Project repository](https://github.com/jqlang/jq)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Stack-buffer-overflow in decNumberCopy Function in jq 1.7.1](https://github.com/jqlang/jq/issues/3196) — Fixed; linked by the maintainer or issue closing event. Evidence: [fix commit](https://github.com/jqlang/jq/commit/a09a4dfd55e6c24d04b35062ccfe4509748b1dd3).

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`a09a4dfd55`](https://github.com/jqlang/jq/commit/a09a4dfd55e6c24d04b35062ccfe4509748b1dd3) | Fix linked to issue #3196: Stack-buffer-overflow in decNumberCopy Function in jq 1.7.1 | Reported bug; maintainer-authored fix |

</details>

### LibreDWG

[Project repository](https://github.com/LibreDWG/libredwg)

<details>
<summary>Pull requests (1)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Fix vuln OSV-2024-384](https://github.com/LibreDWG/libredwg/pull/1061) | Merged | Upstream: `LibreDWG/libredwg` | oss-patch · PatchAgent-assisted |

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`56d392a7e5`](https://github.com/LibreDWG/libredwg/commit/56d392a7e5ae5f522004ff92396dabd468f8d810) | Fix vuln OSV-2024-384 | Authored commit; PatchAgent-assisted |

</details>

### libssh2

[Project repository](https://github.com/libssh2/libssh2)

<details>
<summary>Pull requests (1)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [kex: fix null pointer dereference in `diffie_hellman_sha_algo()`](https://github.com/libssh2/libssh2/pull/1508) | Merged | Upstream: `libssh2/libssh2` | oss-patch · PatchAgent-assisted |

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`1ac1ff4438`](https://github.com/libssh2/libssh2/commit/1ac1ff4438b1f20325768f403755935c94f1b409) | kex.c: fix possible null pointer dereference in diffie_hellman_sha_algo() (#1508) | Authored commit; PatchAgent-assisted |

</details>

### LibTIFF

[Project repository](https://github.com/libsdl-org/libtiff)

The commit links below point to the SDL mirror of [LibTIFF](https://gitlab.com/libtiff/libtiff).

<details>
<summary>Commits and patchsets (5)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`534ac46244`](https://github.com/libsdl-org/libtiff/commit/534ac46244a4ba39c5c490bb65df77619bca927b) | thumbnail: improve integer overflow check for image memory allocation | Authored commit |
| [`721905b0ca`](https://github.com/libsdl-org/libtiff/commit/721905b0ca4b7e4c922debf5038d22c4b91e1bfe) | thumbnail: add integer overflow check for image memory allocation | Authored commit |
| [`11acbe5d9d`](https://github.com/libsdl-org/libtiff/commit/11acbe5d9db7bae0ab522968c7d55222d2a94291) | thumbnail: prevent integer overflow by capping row count at 256 | Authored commit |
| [`5f6a9a0ac6`](https://github.com/libsdl-org/libtiff/commit/5f6a9a0ac6f7633cadb4f6444579d35643d805c2) | rgb2ycbcr: fix integer overflow check for pixel count calculation | Authored commit |
| [`30baf44663`](https://github.com/libsdl-org/libtiff/commit/30baf44663a6b2241213e292755520cc4aeab5fc) | thumbnail.c: add error handling for missing strip and tile byte counts | Authored commit |

</details>

### Linux

[Project repository](https://github.com/torvalds/linux)

<details>
<summary>Commits and patchsets (2)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`cafc667982`](https://github.com/torvalds/linux/commit/cafc6679824a026998d93e7435f6005f64e515d2) | jfs: replace hardcoded magic number with DTPAGEMAXSLOT constant | Authored commit; PatchAgent-assisted |
| [`856db37592`](https://github.com/torvalds/linux/commit/856db37592021e9155384094e331e2d4589f28b1) | jfs: fix metapage reference count leak in dbAllocCtl | Authored commit; PatchAgent-assisted |

</details>

### mJS

[Project repository](https://github.com/cesanta/mjs)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Function Pointer Hijack mjs/mjs.c in mjs_execute](https://github.com/cesanta/mjs/issues/250) — Report submitted; no specific accepted fix verified yet.

</details>

### Nokogiri

[Project repository](https://github.com/sparklemotion/nokogiri)

- [GHSA-phwj-rprq-35pp](https://github.com/advisories/GHSA-phwj-rprq-35pp) — Nokogiri: Possible Use-After-Free when setting an attribute value via `Nokogiri::XML::Attr#value=` or `#content=`. Official reporter credit; fixed in 1.19.4.
- [GHSA-wfpw-mmfh-qq69](https://github.com/advisories/GHSA-wfpw-mmfh-qq69) — Nokogiri: Possible Use-After-Free in XInclude Processing. Official reporter credit; fixed in 1.19.4.
- [GHSA-p67v-3w7g-wjg7](https://github.com/advisories/GHSA-p67v-3w7g-wjg7) — Nokogiri: Possible Use-After-Free when directly using `NokogirI::XML::XPathContext` beyond document lifetime. Official reporter credit; fixed in 1.19.4.
- [GHSA-wjv4-x9w8-wm3h](https://github.com/advisories/GHSA-wjv4-x9w8-wm3h) — Nokogiri: Possible Use-After-Free when setting `Document#root=` to an invalid node type. Official reporter credit; fixed in 1.19.4.
- [GHSA-5prr-v3j2-97mh](https://github.com/advisories/GHSA-5prr-v3j2-97mh) — Nokogiri: Possible Out-of-Bounds Read in `Nokogiri::XML::NodeSet#\[\]`. Official reporter credit; fixed in 1.19.4.
- [GHSA-9cv2-cfxc-v4v2](https://github.com/advisories/GHSA-9cv2-cfxc-v4v2) — Nokogiri: Null Pointer Dereference calling methods on uninitialized wrapper classes. Official reporter credit; fixed in 1.19.4.
- [GHSA-5v8h-3h3q-446p](https://github.com/advisories/GHSA-5v8h-3h3q-446p) — Nokogiri: Possible Use-After-Free when `Nokogiri::XML::Document#encoding=` raises an exception. Official reporter credit; fixed in 1.19.4.

### ntopng

[Project repository](https://github.com/ntop/ntopng)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Heap-buffer-overflow in `Flow::dissectMDNS` leading to crash in ntopng 6.2](https://github.com/ntop/ntopng/issues/8793) — Maintainer stated fuzzing works with the latest development version; issue closed as completed. Evidence: [maintainer response](https://github.com/ntop/ntopng/issues/8793#issuecomment-2453968010), [maintainer response](https://github.com/ntop/ntopng/issues/8793#issuecomment-2454924365), [maintainer response](https://github.com/ntop/ntopng/issues/8793#issuecomment-4808543802).

</details>

### Oj

[Project repository](https://github.com/ohler55/oj)

- [GHSA-3v45-f3vh-wg7m](https://github.com/advisories/GHSA-3v45-f3vh-wg7m) — Oj: Stack Buffer Overflow in Oj.dump via Large Indent. Official reporter credit; fixed in 3.17.3.

### open62541

[Project repository](https://github.com/open62541/open62541)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Assertion Failure in `fuzz_binary_decode` Leads to Crash in Open62541 1.4.6](https://github.com/open62541/open62541/issues/6825) — Maintainer reproduced the issue on 1.4.6 and identified an existing fix on the 1.4 branch. Evidence: [fix commit](https://github.com/open62541/open62541/commit/b9473527623125b5ca264dae4551f8cc414b3bc3), [maintainer response](https://github.com/open62541/open62541/issues/6825#issuecomment-2460650733).

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`b947352762`](https://github.com/open62541/open62541/commit/b9473527623125b5ca264dae4551f8cc414b3bc3) | Fix linked to issue #6825: Assertion Failure in `fuzz_binary_decode` Leads to Crash in Open62541 1.4.6 | Reported bug; maintainer-authored fix |

</details>

### OpenWrt LuCI

[Project repository](https://github.com/openwrt/luci)

- [GHSA-jgc3-4q3p-g6xh](https://github.com/openwrt/luci/security/advisories/GHSA-jgc3-4q3p-g6xh) — 2040-bit certificate signing causes a heap buffer overflow in `luci-lib-px5g`. Official reporter credit. Published advisory; patched version not specified.

### PcapPlusPlus

[Project repository](https://github.com/seladb/PcapPlusPlus)

<details>
<summary>Pull requests (3)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Fix vuln OSV-2024-947](https://github.com/seladb/PcapPlusPlus/pull/1699) | Merged | Upstream: `seladb/PcapPlusPlus` | oss-patch · PatchAgent-assisted |
| [Fix vuln OSV-2024-343](https://github.com/seladb/PcapPlusPlus/pull/1680) | Merged | Upstream: `seladb/PcapPlusPlus` | oss-patch · PatchAgent-assisted |
| [Fix Heap-buffer-overflow in __parse_options](https://github.com/seladb/PcapPlusPlus/pull/1678) | Merged | Upstream: `seladb/PcapPlusPlus` | oss-patch · PatchAgent-assisted |

</details>

<details>
<summary>Commits and patchsets (3)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`132c9cf005`](https://github.com/seladb/PcapPlusPlus/commit/132c9cf00500e691995a49e08bd68a96a095e76e) | Fix vuln OSV-2024-947 (#1699) | Authored commit; PatchAgent-assisted |
| [`a9e823951e`](https://github.com/seladb/PcapPlusPlus/commit/a9e823951efa2aca929f09b0f842f902ce28249d) | Fix Heap-buffer-overflow in __parse_options (#1678) | Authored commit; PatchAgent-assisted |
| [`bc5c08d3df`](https://github.com/seladb/PcapPlusPlus/commit/bc5c08d3df37e9d725656c345d3991ab0c982717) | Fix vuln OSV-2024-343 (#1680) | Authored commit; PatchAgent-assisted |

</details>

### PCL

[Project repository](https://github.com/PointCloudLibrary/pcl)

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Uncaught Exception in PCLPointCloud2::at When Parsing Malformed PLY Files (Potential DoS Vulnerability)](https://github.com/PointCloudLibrary/pcl/issues/6162) — Fixed by an upstream merged PR. Evidence: [fix PR](https://github.com/PointCloudLibrary/pcl/pull/6179), [fix commit](https://github.com/PointCloudLibrary/pcl/commit/a4ad614a1587801092fd085e4796c411017a77ac), [maintainer response](https://github.com/PointCloudLibrary/pcl/issues/6162#issuecomment-2453448952), [maintainer response](https://github.com/PointCloudLibrary/pcl/issues/6162#issuecomment-2453464810).

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`a4ad614a15`](https://github.com/PointCloudLibrary/pcl/commit/a4ad614a1587801092fd085e4796c411017a77ac) | Misc small fixes and improvements | Reported bug; maintainer-authored fix |

</details>

### PHP

[Project repository](https://github.com/php/php-src)

<details>
<summary>Pull requests (1)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Fix unreachable code in URL output handler](https://github.com/php/php-src/pull/19056) | Merged | Upstream: `php/php-src` | cla7aye15I4nd |

</details>

<details>
<summary>Bug and vulnerability reports (1)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Heap Use-After-Free (UAF) Bug in PHP](https://github.com/php/php-src/issues/16726) — Maintainer confirmed the UAF as a bug, but explicitly did not classify it as a security vulnerability; still open. Evidence: [maintainer response](https://github.com/php/php-src/issues/16726#issuecomment-2463078282), [maintainer response](https://github.com/php/php-src/issues/16726#issuecomment-2464803664), [maintainer response](https://github.com/php/php-src/issues/16726#issuecomment-2464848004), [maintainer response](https://github.com/php/php-src/issues/16726#issuecomment-2465235800).

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`b068ee307f`](https://github.com/php/php-src/commit/b068ee307f3185ecd4d2a2f476c005bcc24e873a) | Fix unreachable code in URL output handler (#19056) | Authored commit |

</details>

### Python

[Project repository](https://github.com/python/cpython)

<details>
<summary>Pull requests (1)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [gh-122431: update error message for negative nelements in readline_append_h…](https://github.com/python/cpython/pull/143075) | Merged | Upstream: `python/cpython` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`a273bc99d2`](https://github.com/python/cpython/commit/a273bc99d2ff853f59ee6da4d897b1be72a03975) | gh-122431: Correct the non-negative error message in `readline.append_history_file` (GH-143075) | Authored commit |

</details>

### Qiling

[Project repository](https://github.com/qilingframework/qiling)

<details>
<summary>Pull requests (38)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Refactor MCU module](https://github.com/qilingframework/qiling/pull/1101) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add Arduino Due (SAM3X8E) Support](https://github.com/qilingframework/qiling/pull/1089) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add stm32f103 support](https://github.com/qilingframework/qiling/pull/1087) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Some fix for ARM exception handler and mnist example](https://github.com/qilingframework/qiling/pull/1056) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Some STM32 updates](https://github.com/qilingframework/qiling/pull/1040) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add a simple OLED12864 render and example](https://github.com/qilingframework/qiling/pull/1034) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add more peripheral support for STM32F4](https://github.com/qilingframework/qiling/pull/1028) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add riscv MCU support and update the argument setting](https://github.com/qilingframework/qiling/pull/1008) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add riscv32 dynamic-link elf support](https://github.com/qilingframework/qiling/pull/998) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Refactor the core setup function to support the RISC-V MCU](https://github.com/qilingframework/qiling/pull/994) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Handle the dir_fd argument of stat syscall](https://github.com/qilingframework/qiling/pull/990) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Preparation for gd32 peripheral](https://github.com/qilingframework/qiling/pull/985) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Fix some error handler in posix syscall](https://github.com/qilingframework/qiling/pull/981) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Introduce “riscv” architecture to qiling](https://github.com/qilingframework/qiling/pull/980) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Update the system call mapping style](https://github.com/qilingframework/qiling/pull/978) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Avoid scanning the entire syscall table](https://github.com/qilingframework/qiling/pull/977) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add "external device" module and LCD1602](https://github.com/qilingframework/qiling/pull/972) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add connectivity peripheral's base class](https://github.com/qilingframework/qiling/pull/971) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Added some peripheral details](https://github.com/qilingframework/qiling/pull/969) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Refactor the peripheral logger mechanism and handle the interrupt crash](https://github.com/qilingframework/qiling/pull/968) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Fix the USART debug output](https://github.com/qilingframework/qiling/pull/960) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add a stm32f407 testcase from example](https://github.com/qilingframework/qiling/pull/953) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add support for STM32 series microcontroller simulation](https://github.com/qilingframework/qiling/pull/940) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add a LCD Advance Example](https://github.com/qilingframework/rootfs/pull/24) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add SPI simple test](https://github.com/qilingframework/rootfs/pull/23) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add I2C-LCD testcase](https://github.com/qilingframework/rootfs/pull/22) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add DMA and Timer testcase](https://github.com/qilingframework/rootfs/pull/21) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Recompile the FreeRTOS testcase with shorter sleep time](https://github.com/qilingframework/rootfs/pull/20) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add FreeRTOS as MCU test](https://github.com/qilingframework/rootfs/pull/19) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add stm32f407 example](https://github.com/qilingframework/rootfs/pull/17) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add a 'md5 server' as system test for usart i/o](https://github.com/qilingframework/rootfs/pull/14) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add uart testcase for stm32f4](https://github.com/qilingframework/rootfs/pull/11) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add a simple STM32 example](https://github.com/qilingframework/rootfs/pull/9) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add ping-test's binary and dependent libraries](https://github.com/qilingframework/rootfs/pull/5) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Improve network system call, '/bin/ping' can works now](https://github.com/qilingframework/qiling/pull/838) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add cloexec test binary](https://github.com/qilingframework/rootfs/pull/4) | Merged | Upstream: `qilingframework/rootfs` | cla7aye15I4nd |
| [Add basic support for the close-on-exec flag](https://github.com/qilingframework/qiling/pull/835) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |
| [Add some relocation types (x86)](https://github.com/qilingframework/qiling/pull/827) | Merged | Upstream: `qilingframework/qiling` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (581)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`5dad11a0ee`](https://github.com/qilingframework/qiling/commit/5dad11a0ee40c2264fe5afc58a4b3578175324df) | Fix return type missing | Authored commit |
| [`357815d8e9`](https://github.com/qilingframework/qiling/commit/357815d8e9bdb777228490e6ce7c8c1379901880) | Merge remote-tracking branch 'origin/dev' into next | Authored commit |
| [`0772ddef4b`](https://github.com/qilingframework/qiling/commit/0772ddef4b61e3c7f7d45ce12fa39c5cac827b43) | Merge branch 'qilingframework:master' into next | Authored commit |
| [`d697f5d292`](https://github.com/qilingframework/qiling/commit/d697f5d29287d61bbf5eedfe61eb5bee063db92e) | Fix a typo | Authored commit |
| [`7547918d0d`](https://github.com/qilingframework/qiling/commit/7547918d0d9411929e074d098bb9e8d8b14c58a0) | Tune counter method | Authored commit |
| [`c3a419165a`](https://github.com/qilingframework/qiling/commit/c3a419165a5cbb8367fa943727fc7a4213cdd826) | Change log level | Authored commit |
| [`5b5540e155`](https://github.com/qilingframework/qiling/commit/5b5540e155440c029b7e10ccb45335fd60ed01d1) | Merge branch 'dev' into next | Authored commit |
| [`e2ec8014ef`](https://github.com/qilingframework/qiling/commit/e2ec8014ef6116b379e5c45eac80b24aca8acbf5) | Fix the MCU fuzzer | Authored commit |
| [`d9af57d4db`](https://github.com/qilingframework/qiling/commit/d9af57d4db5b6beba307a60712e1da87664f52d1) | Merge branch 'dev' into next | Authored commit |
| [`b6a697dca2`](https://github.com/qilingframework/qiling/commit/b6a697dca270d22485e1b781b1a36e4165323849) | Merge 'dev' into next | Authored commit |
| [`8b05c8c4e4`](https://github.com/qilingframework/qiling/commit/8b05c8c4e4559518610091e77d1314da423b814e) | Faster UART ? | Authored commit |
| [`ed0e70d3b0`](https://github.com/qilingframework/qiling/commit/ed0e70d3b0e5e5f08479ac30666f14ee299001d7) | Update rootfs | Authored commit |
| [`cb9e58f23e`](https://github.com/qilingframework/qiling/commit/cb9e58f23ede6603d079f4c4aae492b7b48be8e3) | Update fuzz script | Authored commit |
| [`abf2ad3821`](https://github.com/qilingframework/qiling/commit/abf2ad3821f19f289863ac3d5d93cb7376548fff) | Add fast mode in MCU | Authored commit |
| [`1a838bda64`](https://github.com/qilingframework/qiling/commit/1a838bda643673c0e330696bf1af9eb3bc3b3afe) | Delete unicorn task in arch | Authored commit |
| [`797ca44007`](https://github.com/qilingframework/qiling/commit/797ca44007a3d42b45e2efee67c46d50b0270461) | Change log level for missing peripheral | Authored commit |
| [`df1046d784`](https://github.com/qilingframework/qiling/commit/df1046d7846d776b5584c9c10feb782eb910883d) | Add fast_mode in QlOsMcu | Authored commit |
| [`e1973bf7d3`](https://github.com/qilingframework/qiling/commit/e1973bf7d3f1cfab18c8ccb4a2106443ce6a8d20) | A very slow fuzzer | Authored commit |
| [`ee02d7c0af`](https://github.com/qilingframework/qiling/commit/ee02d7c0af05cbf7dd95c644d402c92d53ebfede) | Add hackme testcase | Authored commit |
| [`6adf08994f`](https://github.com/qilingframework/qiling/commit/6adf08994f47abec0b01bce86679e3b3264f57f3) | Update rootfs | Authored commit |
| [`e5dd9c16bb`](https://github.com/qilingframework/qiling/commit/e5dd9c16bb67e1a16036ba122c9c6733e2e25315) | Add save/store for connectivity peripheral | Authored commit |
| [`f232deef95`](https://github.com/qilingframework/qiling/commit/f232deef95abf170946ede3f24d5fb1fca0a39c7) | Add ql_afl_fuzz_custom in __init__ | Authored commit |
| [`0fba67db88`](https://github.com/qilingframework/qiling/commit/0fba67db887d00df1ed52ed76099ae768c1aabcb) | Add grain size control | Authored commit |
| [`64ab6e5e25`](https://github.com/qilingframework/qiling/commit/64ab6e5e254a33cd68558a685cac400857c66b32) | Add stepable check | Authored commit |
| [`1807f2981e`](https://github.com/qilingframework/qiling/commit/1807f2981e89d674c07fc96c71ec0efe1d0561d3) | Modify hw.attr api | Authored commit |
| [`96b960c1da`](https://github.com/qilingframework/qiling/commit/96b960c1da9882249b5e838a848ff69acf81dcbc) | Delete debug print | Authored commit |
| [`7a84f106b0`](https://github.com/qilingframework/qiling/commit/7a84f106b04bdafff2a4d554900df9bcc65a2eb9) | Simplify interrupt handler | Authored commit |
| [`461ac52334`](https://github.com/qilingframework/qiling/commit/461ac523346ce89bc375f11aad3edabf1e198105) | Optimize the peripherial step method | Authored commit |
| [`08c01c0d26`](https://github.com/qilingframework/qiling/commit/08c01c0d26961e58c648fbd1a13023071f79f6c1) | Merge branch 'dev' into next | Authored commit |
| [`225175caf3`](https://github.com/qilingframework/qiling/commit/225175caf36e654194aadbf04ed79c012e0ef2a0) | Merge branch 'dev' into next | Authored commit |
| [`efbb78b469`](https://github.com/qilingframework/qiling/commit/efbb78b469bf9d256c37400aad85006691adf2d1) | Update rootfs | Authored commit |
| [`77c4e1ab04`](https://github.com/qilingframework/qiling/commit/77c4e1ab047518f35d7f7952e048485bbc5856bf) | Delete read in sd | Authored commit |
| [`8446882a17`](https://github.com/qilingframework/qiling/commit/8446882a17f71dd77ebd195d454797807dcbf1eb) | Add SDIO logic | Authored commit |
| [`e9d3a6a661`](https://github.com/qilingframework/qiling/commit/e9d3a6a661b89b23f11cfd3b73b061c96df39226) | Add MK64F12 FlexTimer | Authored commit |
| [`28e6dcf8cd`](https://github.com/qilingframework/qiling/commit/28e6dcf8cdce67c1217834ebd9136ff707b1b5fa) | Add mk64f12 timer | Authored commit |
| [`fd1e92ac5b`](https://github.com/qilingframework/qiling/commit/fd1e92ac5bdc6aeaffea99184e4e5139b727af5f) | Fix spi recv logic | Authored commit |
| [`4aa6bde2ee`](https://github.com/qilingframework/qiling/commit/4aa6bde2ee9e6a4f922f593bf6fd2b42dc2671ce) | Add MK64F12 SPI | Authored commit |
| [`f756294f81`](https://github.com/qilingframework/qiling/commit/f756294f817d073ecec490013e688e96215ac2c6) | Fix pwr setup logic | Authored commit |
| [`88492e6373`](https://github.com/qilingframework/qiling/commit/88492e6373eebdd77b1b26a83841bc234919b4e4) | Fix UART setting | Authored commit |
| [`2afe98d884`](https://github.com/qilingframework/qiling/commit/2afe98d884496187e791f594bb5866eed57c025b) | Delete a wrong testcase (The firmware is wrong) | Authored commit |
| [`72ea05024f`](https://github.com/qilingframework/qiling/commit/72ea05024ff88bf5ee0d6205f0b52a0228bacc3d) | Simplify USART Logic | Authored commit |
| [`8b504ac5b9`](https://github.com/qilingframework/qiling/commit/8b504ac5b9a8d5c4668d1239c3f762ea2828a19f) | Fix systick interrupt bug | Authored commit |
| [`191b308977`](https://github.com/qilingframework/qiling/commit/191b3089771f133d1c00a13c66640a688b15feed) | Merge branch 'dev' into next | Authored commit |
| [`812ede98d5`](https://github.com/qilingframework/qiling/commit/812ede98d5d436bc16e3e6599760565f86cde5b0) | Fix GPIO input mach | Authored commit |
| [`8b9ec29a51`](https://github.com/qilingframework/qiling/commit/8b9ec29a514fb86d44d3a5efcfa1a085ef7b68d6) | Add stm32f4xxDac | Authored commit |
| [`ad23467b5e`](https://github.com/qilingframework/qiling/commit/ad23467b5ee3b36a67b72aef03cf0db9b4690de4) | Fix spi receiver | Authored commit |
| [`20bedee78d`](https://github.com/qilingframework/qiling/commit/20bedee78d97f8b8c2fe87dbba9e8d2ace12e91a) | Fix timer interrupt handler | Authored commit |
| [`1e6aa4e2b7`](https://github.com/qilingframework/qiling/commit/1e6aa4e2b7ec61bd26300017936918372a262d13) | Fix stm32f4 timer arguments config | Authored commit |
| [`abf25b2781`](https://github.com/qilingframework/qiling/commit/abf25b278182ceb31821ccdadda95f409203790e) | Simplify stm32 timer interrupts | Authored commit |
| [`ead99f69b3`](https://github.com/qilingframework/qiling/commit/ead99f69b3e0dd6995be7778c1ed42f1c5fbfafe) | Add STM32F1 ADC logic | Authored commit |
| [`45f40aa7f0`](https://github.com/qilingframework/qiling/commit/45f40aa7f076a95aa845484ab1d4214cb5bc4150) | Fix a UART receive bug | Authored commit |
| [`f1b875d193`](https://github.com/qilingframework/qiling/commit/f1b875d193bee674c8f8c24c193bc4bc6bf5d994) | Add MK64F12 UART Interrupt | Authored commit |
| [`75431d0a9c`](https://github.com/qilingframework/qiling/commit/75431d0a9c54199c37be4b15b8f4bd486b009b3c) | Fix data register field size | Authored commit |
| [`707d125c30`](https://github.com/qilingframework/qiling/commit/707d125c300add93e69673125c6ae21154449758) | Add Transmiter and Receiver into spi | Authored commit |
| [`a481d4fa6d`](https://github.com/qilingframework/qiling/commit/a481d4fa6dab61e14a4e67ebeb4cecc16371c00b) | Add "push button" interrupt | Authored commit |
| [`f13567a630`](https://github.com/qilingframework/qiling/commit/f13567a6301b6bf49105572f103244c62f736b03) | Add MK64F12 port const | Authored commit |
| [`cbc23e7472`](https://github.com/qilingframework/qiling/commit/cbc23e747225a5225522686d1fdbdcaaf864c653) | Connect gpio and port | Authored commit |
| [`914fb429e4`](https://github.com/qilingframework/qiling/commit/914fb429e417f5225f28df4ff2d87c1a444d3908) | Fix typo of PORT | Authored commit |
| [`8fd72da778`](https://github.com/qilingframework/qiling/commit/8fd72da7787e3a8ff0e5f0a16d11b60d0971dc0b) | Add toggle mach in gpio | Authored commit |
| [`8e57fa4b43`](https://github.com/qilingframework/qiling/commit/8e57fa4b434a0ab8be0039a219a7ce7503540f75) | Fix MK64F12 Port Structure | Authored commit |
| [`15bee55110`](https://github.com/qilingframework/qiling/commit/15bee55110c41ad0c1bae7ac81eb7db6c671181c) | Add MK64F12 GPIO setting | Authored commit |
| [`280322a833`](https://github.com/qilingframework/qiling/commit/280322a833acf41a2a2258b5eb52cad5554a8deb) | Add MK64F12 Real Time Clock | Authored commit |
| [`1170283dea`](https://github.com/qilingframework/qiling/commit/1170283deaa2a6858fc9dc1fc2d167e012e0d1e5) | Add MK64F12 System Controller | Authored commit |
| [`749a4225ee`](https://github.com/qilingframework/qiling/commit/749a4225eeb1ea718734299adb44d4665ba2746b) | Add MK64F12 GPIO | Authored commit |
| [`8dabd602fd`](https://github.com/qilingframework/qiling/commit/8dabd602fd94dc7863ec8e9a38ba8957402eac7c) | Add MK64F12 ADC Logic | Authored commit |
| [`8ad0eea28f`](https://github.com/qilingframework/qiling/commit/8ad0eea28f8a94bc0ed119287c7a60d42866be43) | Fix MK64F12 GPIO keyword arguments | Authored commit |
| [`8715a9e23b`](https://github.com/qilingframework/qiling/commit/8715a9e23b8b00cedfb9a7d44818935e915278e4) | Add kinetis BME mach | Authored commit |
| [`2180b63830`](https://github.com/qilingframework/qiling/commit/2180b63830f1636a5cd0ae535cfc5daa798bc125) | Add BME Entry | Authored commit |
| [`46eddfb8d6`](https://github.com/qilingframework/qiling/commit/46eddfb8d6d1d41a4b1199e864726c5dc2040359) | Fix some logic, but it may be wrong | Authored commit |
| [`737dd08dbf`](https://github.com/qilingframework/qiling/commit/737dd08dbf0d9a23d58e978761e4f6480c57cd7f) | Add bitband region for MK64F12 | Authored commit |
| [`3ef6eae0ad`](https://github.com/qilingframework/qiling/commit/3ef6eae0ad0e58a4cbc1fc852415311b25592ab5) | Merge branch 'dev' into next | Authored commit |
| [`27764ce799`](https://github.com/qilingframework/qiling/commit/27764ce7999c393ed64c5bd6396412902a5943d0) | Fix bitband in Arduino Due | Authored commit |
| [`b81ddb50db`](https://github.com/qilingframework/qiling/commit/b81ddb50db9a67e26c3a84aca04e4739e094ec5c) | Fix remap in Arduino Due | Authored commit |
| [`163b28c345`](https://github.com/qilingframework/qiling/commit/163b28c345e74814ea10f9b8f7ba8418bce8c8c2) | Add MemoryRemap peripheral | Authored commit |
| [`c9ae1b79e1`](https://github.com/qilingframework/qiling/commit/c9ae1b79e1abe5b76fe00d43c246baae6f5fb363) | Remove setup_remap | Authored commit |
| [`40763bb471`](https://github.com/qilingframework/qiling/commit/40763bb471dd870ec39c8f723d041b25072e3b15) | Move remap into peripheral | Authored commit |
| [`fda6977a0c`](https://github.com/qilingframework/qiling/commit/fda6977a0c2a53f11da7459b86c66d8ec18ca47a) | Change bitband into peripheral in config | Authored commit |
| [`2b9bb8195c`](https://github.com/qilingframework/qiling/commit/2b9bb8195cfe07c47fa6df2e95c7d68333356178) | Move bitband into peripheral | Authored commit |
| [`31a0b019f2`](https://github.com/qilingframework/qiling/commit/31a0b019f267423852a9d126ca0390ef68188777) | Delete setup_bitband in hw | Authored commit |
| [`14a351580c`](https://github.com/qilingframework/qiling/commit/14a351580c6e5332629496da5cc515ae2ea8d802) | Do not need load bitband anymore | Authored commit |
| [`23069f89d4`](https://github.com/qilingframework/qiling/commit/23069f89d46a70df33eb379bb4c96deb562d7807) | Delete re-profile testcase | Authored commit |
| [`8f5a6c3109`](https://github.com/qilingframework/qiling/commit/8f5a6c3109ba8388cf176cd0ad2e5c14599d18f9) | Move some peripheral into misc | Authored commit |
| [`16f18ed93a`](https://github.com/qilingframework/qiling/commit/16f18ed93a412fea70041bbc7ec24fc43e0a843f) | Add basic logic for K64F UART | Authored commit |
| [`043f0645ad`](https://github.com/qilingframework/qiling/commit/043f0645adda363bf8c80debd7a76d1eabca132b) | Add MK64F12 Mcg logic | Authored commit |
| [`86f4f52607`](https://github.com/qilingframework/qiling/commit/86f4f526077808b4fdda50b7d66dd2fe539d39b4) | Fix some pio bugs | Authored commit |
| [`9c21628b2e`](https://github.com/qilingframework/qiling/commit/9c21628b2e87eab9931127ef68822b8e17369d0d) | Add SAM3XA SPI Testcase | Authored commit |
| [`386d75c627`](https://github.com/qilingframework/qiling/commit/386d75c6278842292e89a1cdeeb4f83eb4031c94) | Add Arduino Due PWM Test | Authored commit |
| [`4964fc5098`](https://github.com/qilingframework/qiling/commit/4964fc50983575a7b29fa49a5b7ed59ff84e791a) | Fix some pio bugs | Authored commit |
| [`2cc121f533`](https://github.com/qilingframework/qiling/commit/2cc121f53378bc1b505d9e7845b73bb74634523b) | Enable GPIO set/reset in SAM3XA | Authored commit |
| [`bbde87d34e`](https://github.com/qilingframework/qiling/commit/bbde87d34e79bcebba88d128f55fd19b89f7331e) | Add sam3xa dac | Authored commit |
| [`9118e7651d`](https://github.com/qilingframework/qiling/commit/9118e7651dd7ef0dbbe03345f347af9574a89ca9) | Fix sam3x8e peripheral name | Authored commit |
| [`8eeb421261`](https://github.com/qilingframework/qiling/commit/8eeb421261e65cde2f148cff809d6ff0bc974fd6) | Change folder name | Authored commit |
| [`fca2c92c20`](https://github.com/qilingframework/qiling/commit/fca2c92c2057c8b233a89620f4c4ce13f79f780b) | Fix some adc logic | Authored commit |
| [`9ce288ad79`](https://github.com/qilingframework/qiling/commit/9ce288ad79ca56452d93551bdee0623e5c68a414) | Fix Arduino Due UART Logic | Authored commit |
| [`39dd755965`](https://github.com/qilingframework/qiling/commit/39dd7559651132ea33fc9271045231722e76f4eb) | Fix wrong import | Authored commit |
| [`63f58eb1eb`](https://github.com/qilingframework/qiling/commit/63f58eb1eb5bb6767ec23366e88100d51e7b3c92) | Add some eth logics | Authored commit |
| [`33437addf5`](https://github.com/qilingframework/qiling/commit/33437addf50db16146910fe42cc44988ad6ee663) | Add raw read/write api | Authored commit |
| [`be3d3641d2`](https://github.com/qilingframework/qiling/commit/be3d3641d22c4d73355df0a2f7744a61ef0320a8) | Add K64F Adc struct | Authored commit |
| [`c9e981a474`](https://github.com/qilingframework/qiling/commit/c9e981a47430a8fd6b693b42501c46efe1eb6fb2) | Add MK64F12 UART Struct | Authored commit |
| [`dd73598654`](https://github.com/qilingframework/qiling/commit/dd735986542f2cd91e9bd0e18a5eda37e13a466b) | Merge branch 'dev' into next | Authored commit |
| [`407f1fa4f2`](https://github.com/qilingframework/qiling/commit/407f1fa4f200be61fb188047fdd51cfd17a1892e) | Fix default peripheral read/write function | Authored commit |
| [`6f817c9c6c`](https://github.com/qilingframework/qiling/commit/6f817c9c6cbe67933cd219dc6ee98c159f5d11b8) | Add save/store for timer | Authored commit |
| [`10665ee99e`](https://github.com/qilingframework/qiling/commit/10665ee99e4567ec37a9d660ff419ae6fd727233) | Fix ctypes save/restore bug | Authored commit |
| [`2e3502753e`](https://github.com/qilingframework/qiling/commit/2e3502753e22f87f1c8332761413ac020c78c975) | Fix count bug in QlOsMcu | Authored commit |
| [`07525006bb`](https://github.com/qilingframework/qiling/commit/07525006bb957322ae6b5213e9b35e41c5c33e52) | Refactor peripheral hook | Authored commit |
| [`2add022b1a`](https://github.com/qilingframework/qiling/commit/2add022b1afa93ad5337fbbbff657c29c158ca7d) | Rename Op to Action | Authored commit |
| [`85ab1f3071`](https://github.com/qilingframework/qiling/commit/85ab1f3071b0d785c9c230b980553758a2470069) | Fix peripheral hook paramater | Authored commit |
| [`36c8f42316`](https://github.com/qilingframework/qiling/commit/36c8f423164d558df0e5634da1b7a5fbf2bc5131) | Add snapshot test | Authored commit |
| [`cb08f973fd`](https://github.com/qilingframework/qiling/commit/cb08f973fdc0baebc45e8b9ea6bd455e39cb12f8) | Implement qiling save/restore | Authored commit |
| [`ed19f5c5c0`](https://github.com/qilingframework/qiling/commit/ed19f5c5c0dc183ef16ab057a6ec8e7e30792688) | Add default instance | Authored commit |
| [`6348001ed0`](https://github.com/qilingframework/qiling/commit/6348001ed06fae90e33fc9b78666a3330573f1b1) | Replace timer with instance | Authored commit |
| [`56fc4aad5d`](https://github.com/qilingframework/qiling/commit/56fc4aad5dd2e87c6e3cfdc3e44667f28e01431d) | Fix replace bug again | Authored commit |
| [`1cf8f14df3`](https://github.com/qilingframework/qiling/commit/1cf8f14df3ec50b5b1bd48b844982bca14c4310b) | Fix replace bug | Authored commit |
| [`a34ad72697`](https://github.com/qilingframework/qiling/commit/a34ad72697ae0aa0f6aaf2847f41fb3e14d97ecb) | Replace spi with instance | Authored commit |
| [`adaf89a7d9`](https://github.com/qilingframework/qiling/commit/adaf89a7d98fe49fa590b2558fec4a0bd2857da9) | Replace timer with instance | Authored commit |
| [`f417050b47`](https://github.com/qilingframework/qiling/commit/f417050b47b3b02fb909da8dbfc16ae802b68e25) | Replace timer with instance | Authored commit |
| [`865242c278`](https://github.com/qilingframework/qiling/commit/865242c27842f3d7641fa3cf21b237f61da720d9) | Replace spi with instance | Authored commit |
| [`6ba651c3b4`](https://github.com/qilingframework/qiling/commit/6ba651c3b4a921ff01739e689cb44467cc4bf1a9) | Replace sd with instance | Authored commit |
| [`b8929772b6`](https://github.com/qilingframework/qiling/commit/b8929772b60d76bb57ea2115ae0336617cad6e80) | Replace pwr with instance | Authored commit |
| [`05bfec5676`](https://github.com/qilingframework/qiling/commit/05bfec567668d33de4cb297c6c5086d33c600cbe) | Replace eth with instance | Authored commit |
| [`b920bf2e16`](https://github.com/qilingframework/qiling/commit/b920bf2e16491531966fb4d0e2561ed7d3b96353) | Replace misc with instance | Authored commit |
| [`21c770dd6b`](https://github.com/qilingframework/qiling/commit/21c770dd6b7cef40429878f82cb90aaadded1ea9) | Replace scb with instance | Authored commit |
| [`0d75d98ac7`](https://github.com/qilingframework/qiling/commit/0d75d98ac7241e0ff695c5aaa72d6f86a4d85562) | Replace crc with instance | Authored commit |
| [`a84d5a1750`](https://github.com/qilingframework/qiling/commit/a84d5a17508b5fb134c8416e9abc6cc1c5824200) | Replace intc with instance | Authored commit |
| [`39d0120c01`](https://github.com/qilingframework/qiling/commit/39d0120c0191ddbdb7d99795c64342deeb4dced8) | Replace i2c with instance | Authored commit |
| [`85b92c0ca9`](https://github.com/qilingframework/qiling/commit/85b92c0ca98a487dbe352ba48273c599af8b4a6b) | Replace gpio with instance | Authored commit |
| [`cc47c0ae83`](https://github.com/qilingframework/qiling/commit/cc47c0ae83c872f3caf4dbfa58ed392e8d470af1) | Replace flash with instance | Authored commit |
| [`d854ac707c`](https://github.com/qilingframework/qiling/commit/d854ac707cf9fe39b29edb3510cfebdf38fbeaff) | Replace dma with instance | Authored commit |
| [`b61d121fab`](https://github.com/qilingframework/qiling/commit/b61d121fab3d5bac5951ad65a97895c85820598e) | Replace char with instance | Authored commit |
| [`5af2728df3`](https://github.com/qilingframework/qiling/commit/5af2728df34cef64b32a9edcae888cc349f399cd) | Replace adc with instance | Authored commit |
| [`d72fd5dfee`](https://github.com/qilingframework/qiling/commit/d72fd5dfee2735f387021bbeffec42f62bfc15ae) | Prepare to add save/restore in MCU | Authored commit |
| [`72819f5bec`](https://github.com/qilingframework/qiling/commit/72819f5beca18f3aa868f14d108646386d0a9e44) | Handle overlapped MMIO | Authored commit |
| [`5a9f49c31e`](https://github.com/qilingframework/qiling/commit/5a9f49c31e2244b007ae8c85e8555c5457a33ab3) | Fix ETH peripheral | Authored commit |
| [`bcc4d74282`](https://github.com/qilingframework/qiling/commit/bcc4d74282fc8287f31ceb01b82be2d56cbbab31) | Fix stm32f429 config's memory size | Authored commit |
| [`8a71685d46`](https://github.com/qilingframework/qiling/commit/8a71685d4681e284622a160701798a847dc21a8f) | Add STM32F4xx eth | Authored commit |
| [`5214ee5b46`](https://github.com/qilingframework/qiling/commit/5214ee5b46ad1c09fb594cc942ec56e6ee666560) | Fix ihexparser bug | Authored commit |
| [`36a7d2c8c6`](https://github.com/qilingframework/qiling/commit/36a7d2c8c677cd2af8a1f2fea33a0e8a1a389f37) | Fix peripheral hook erase bug | Authored commit |
| [`5f7e34f623`](https://github.com/qilingframework/qiling/commit/5f7e34f6238cbaf21dfd2f180891af4ad1fb7004) | Add full support for peripheral hook | Authored commit |
| [`ab4ff10b81`](https://github.com/qilingframework/qiling/commit/ab4ff10b816a654fdbaf15788ecb32298f11fd35) | Delete debug callback MCU examples | Authored commit |
| [`d4e6761f5b`](https://github.com/qilingframework/qiling/commit/d4e6761f5bc84658dde3316e45350d979136d80b) | Merge branch 'dev' into next | Authored commit |
| [`9d72998aa1`](https://github.com/qilingframework/qiling/commit/9d72998aa10b93ba3d2b3cd1b0ad807dc88a3152) | Add mk64f12 sim peripheral | Authored commit |
| [`a362b71e00`](https://github.com/qilingframework/qiling/commit/a362b71e0062bd223d012ee2974d9663f88baaab) | Add Basic NXP peripheral | Authored commit |
| [`1b7f11afb5`](https://github.com/qilingframework/qiling/commit/1b7f11afb5a44a5fca476a1b6e751027a9da9d41) | Add FRDM-K64 board (NXP) | Authored commit |
| [`d793a072f2`](https://github.com/qilingframework/qiling/commit/d793a072f2b5fd0d74635387c36187b775b22de6) | Fix cm4 scb struct | Authored commit |
| [`e6708f47aa`](https://github.com/qilingframework/qiling/commit/e6708f47aae739773686351c1dd8add5d4352457) | Fix stm32f4xx I2C Logic | Authored commit |
| [`5be461963d`](https://github.com/qilingframework/qiling/commit/5be461963d203d4b2a8ac98fde70a6bf5316e620) | Fix pio logic | Authored commit |
| [`454887bd7f`](https://github.com/qilingframework/qiling/commit/454887bd7f86edda6ac2456af8d79344a4eb503a) | Add more timer peripheral | Authored commit |
| [`366a0d2a8f`](https://github.com/qilingframework/qiling/commit/366a0d2a8f7fa3a41d4a10d3404b939f66d2b639) | Add stm32f1xx adx | Authored commit |
| [`d09d0b7f5d`](https://github.com/qilingframework/qiling/commit/d09d0b7f5da46b8b557e2d8dc5af126a1f338503) | Add stm32f1xx spi | Authored commit |
| [`200bfa8ff3`](https://github.com/qilingframework/qiling/commit/200bfa8ff365376345a7c0d998cc2e8dadd44792) | Add SAM3xA const | Authored commit |
| [`893029e733`](https://github.com/qilingframework/qiling/commit/893029e7334ed79c575d4633401f378692dd9bd5) | Add SAM3xA ADC | Authored commit |
| [`6c72ac3265`](https://github.com/qilingframework/qiling/commit/6c72ac3265f39e73bd39875943c4e4287256e04e) | Add load_all api in hw | Authored commit |
| [`556757968e`](https://github.com/qilingframework/qiling/commit/556757968eb5f20ddc4cda026bcc20dc9a1cfb92) | Add stm32f1xx i2c | Authored commit |
| [`cfb48a913e`](https://github.com/qilingframework/qiling/commit/cfb48a913e5a6540bcef84f610a5e9fe9b83a6dc) | Fix `ql.hw.create` arguments meaning | Authored commit |
| [`312442fbd2`](https://github.com/qilingframework/qiling/commit/312442fbd2c5ee70c4b3015235d46623c469dc80) | Fix peripheral field description bug | Authored commit |
| [`9cb15e04fe`](https://github.com/qilingframework/qiling/commit/9cb15e04fedf5e44cd99fc004edd84b2cb1dcde5) | Optimize field description function | Authored commit |
| [`bf1776be28`](https://github.com/qilingframework/qiling/commit/bf1776be286cf5e051a3578945d1b3256efa39e5) | Change api name | Authored commit |
| [`7c264c4558`](https://github.com/qilingframework/qiling/commit/7c264c45588d5b07fb429c2550f96c4f9b2db543) | Fixed boundary error in `ql.hw.find` | Authored commit |
| [`e335fa328f`](https://github.com/qilingframework/qiling/commit/e335fa328f2625237149b98fa37a72db1efc2d64) | Fix the verbose setter bug | Authored commit |
| [`ea6fff682d`](https://github.com/qilingframework/qiling/commit/ea6fff682d1d6346964795a7398d66b92b428500) | Simplify ql.run baremetal part | Authored commit |
| [`b12d0f6ed0`](https://github.com/qilingframework/qiling/commit/b12d0f6ed0a07c93ee6208ac8cfac3cf37b72b66) | Simplfy QlOsMcu.run paramater | Authored commit |
| [`0fb37773ad`](https://github.com/qilingframework/qiling/commit/0fb37773addb3c7aec0a0c8ae112a8e9ba4e7948) | Rename interrupt handler | Authored commit |
| [`53828372a4`](https://github.com/qilingframework/qiling/commit/53828372a40216f93c3642d851079f30c52f8052) | Fix the MCU examples' api | Authored commit |
| [`45bd0df46d`](https://github.com/qilingframework/qiling/commit/45bd0df46d746ca41e93f7b4194c02260c8aba1f) | Fix the QlOsMcu | Authored commit |
| [`768635b96c`](https://github.com/qilingframework/qiling/commit/768635b96cbb90e0a6b6cbe16d3ea3706d307a2d) | Merge branch 'dev' into xv6 | Authored commit |
| [`520df69035`](https://github.com/qilingframework/qiling/commit/520df690356bd2ce08657a1d69714d6efd63a0af) | Cleanup RISCV | Authored commit |
| [`5c458291fc`](https://github.com/qilingframework/qiling/commit/5c458291fc1cc972a7ac22fa2f47208109d8be34) | Fix MCU test api | Authored commit |
| [`e416c706e6`](https://github.com/qilingframework/qiling/commit/e416c706e6b4c02b5ac4021bad50ed30e7abf99d) | Move cortex-m control logic into QlOsMcu | Authored commit |
| [`7efb317fd5`](https://github.com/qilingframework/qiling/commit/7efb317fd5f9b76f37b820152bc67f980960a848) | Fix thumb api reference | Authored commit |
| [`7fd5f91d58`](https://github.com/qilingframework/qiling/commit/7fd5f91d5886c439e370f804ee2c1721ee9f9b07) | Cleanup Cortex-M | Authored commit |
| [`e00ee46dec`](https://github.com/qilingframework/qiling/commit/e00ee46decd6bd241caf776c70b12fbb878932ee) | Simplify the thumb related api | Authored commit |
| [`0a6d6e9d9a`](https://github.com/qilingframework/qiling/commit/0a6d6e9d9a19e7fffaa89aa9e68e4caf952f4332) | Add peripheral hook_read/hook_write | Authored commit |
| [`0f29b48d0e`](https://github.com/qilingframework/qiling/commit/0f29b48d0ee6faf78c3decd39048683e18722bb9) | Merge branch 'dev' into sam3x8e | Authored commit |
| [`3a2af8f7e1`](https://github.com/qilingframework/qiling/commit/3a2af8f7e19c169d18b3bb1f02bbfb95ee791e9f) | Update rootfs | Authored commit |
| [`e27e2a26d8`](https://github.com/qilingframework/qiling/commit/e27e2a26d86b8db1934a38f285d888a9a06e15f8) | Fix test_mcu typo | Authored commit |
| [`7bd78c6bc8`](https://github.com/qilingframework/qiling/commit/7bd78c6bc8ce41f77556bb2e584f1933850d5879) | Fix error import | Authored commit |
| [`57d3a34f26`](https://github.com/qilingframework/qiling/commit/57d3a34f266ff9dbb5d66008056d82b93a888d20) | Add sam3x8e board | Authored commit |
| [`ccbe8be1b9`](https://github.com/qilingframework/qiling/commit/ccbe8be1b96e2197e3afe59bf14fc44f8d222f34) | Fix ihex parser loader | Authored commit |
| [`0cf23594e0`](https://github.com/qilingframework/qiling/commit/0cf23594e0a29e357ad09adef224d0bd0c613754) | Add SAM3xa UART | Authored commit |
| [`354dcabecb`](https://github.com/qilingframework/qiling/commit/354dcabecb97b73428fa644d6fc4ccb02ce114c0) | Add SAM3xa PIO (GPIO) | Authored commit |
| [`1c7b126f35`](https://github.com/qilingframework/qiling/commit/1c7b126f35a0e67c6eb9f86f5a9af4bacb43875f) | Add SAM3xa PDC (DMA) | Authored commit |
| [`08fa6e0d7e`](https://github.com/qilingframework/qiling/commit/08fa6e0d7eecb7bbcf089ece7b8c4427e0a7a2e6) | Add SAM3xa char peripheral | Authored commit |
| [`7946bee442`](https://github.com/qilingframework/qiling/commit/7946bee4427c768de48e069023ee7fb3aa2ee709) | Add SAM3xa UOTGHS | Authored commit |
| [`e5a2fe10cf`](https://github.com/qilingframework/qiling/commit/e5a2fe10cf30467675b63e292b66fae7c5beb018) | Add SAM3xa UART | Authored commit |
| [`e4add3c216`](https://github.com/qilingframework/qiling/commit/e4add3c216eb94ff7f7e8cdbd8a803a81765d726) | Add SAM3xa ADC | Authored commit |
| [`1aee3fbcd6`](https://github.com/qilingframework/qiling/commit/1aee3fbcd64e4a07c5f780fd38847dec8ff1ede0) | Add SAM3XA PMC  basic logic | Authored commit |
| [`4760caa4a3`](https://github.com/qilingframework/qiling/commit/4760caa4a3bf4f2063a328275f6a5c67e389eae1) | Add sam3xa efc | Authored commit |
| [`131da6180f`](https://github.com/qilingframework/qiling/commit/131da6180ffe9c0d5cb9a1e5f75e8f44cf3c837b) | Add hw flash type | Authored commit |
| [`9f78885980`](https://github.com/qilingframework/qiling/commit/9f7888598095168b8dee3e8e19261bd6f7834730) | Add sam3xa Power Management Controller | Authored commit |
| [`bb656f8033`](https://github.com/qilingframework/qiling/commit/bb656f803305ac7bde863f8f1a7f91312e00aee5) | Add description for PMC | Authored commit |
| [`25923f4621`](https://github.com/qilingframework/qiling/commit/25923f462156c4038473c3b47ca320358e6fe8c3) | Add sam3xa PMC | Authored commit |
| [`f79bf17ef8`](https://github.com/qilingframework/qiling/commit/f79bf17ef8e1e4c9f676e9703641d028fb1a15aa) | Fix sam3x8e peripheral name typo | Authored commit |
| [`1984a09f20`](https://github.com/qilingframework/qiling/commit/1984a09f20e043ed0d6cf0ed4a01ee5b949689d8) | Add sam3x8e peripheral config | Authored commit |
| [`59500cc519`](https://github.com/qilingframework/qiling/commit/59500cc519a825547078f1bc74a3a149ec2f54d7) | Add sam3x8e memory layout | Authored commit |
| [`89b1a7fa20`](https://github.com/qilingframework/qiling/commit/89b1a7fa2098a62ace3f5455c52824189d37202e) | Add stm32f103 testcase | Authored commit |
| [`2a582f75ed`](https://github.com/qilingframework/qiling/commit/2a582f75ed3fa521e88afcb32ff479595e31ce27) | Fix stm32f4 DMA copy bug | Authored commit |
| [`22339191f3`](https://github.com/qilingframework/qiling/commit/22339191f34e65691f199efadb68c1bc106f034d) | Add stm32f1xx dma | Authored commit |
| [`8f349b5296`](https://github.com/qilingframework/qiling/commit/8f349b529649e1a7f2ce6a0bc5ccee1bbceb0906) | Delete redundant function in DMA | Authored commit |
| [`1c502ecdf4`](https://github.com/qilingframework/qiling/commit/1c502ecdf472f83f5dc23e643607d1acbbffa970) | Delete useless temporary variable | Authored commit |
| [`efb05a3da0`](https://github.com/qilingframework/qiling/commit/efb05a3da01f40a52529951938ec57ed95c60f8f) | Add exti interrupt config | Authored commit |
| [`120da77b8c`](https://github.com/qilingframework/qiling/commit/120da77b8cc2a3f1bb25d7e1f84914927ebdcc6c) | Add exti soft interrupt support | Authored commit |
| [`204e0f9994`](https://github.com/qilingframework/qiling/commit/204e0f99944ddfe609c1b2247af0a55dbef3a437) | Connect afio with exti | Authored commit |
| [`68d236f184`](https://github.com/qilingframework/qiling/commit/68d236f184cf82a25f5556eff52b568a667e2e2b) | Unity stm32f1/4 gpio | Authored commit |
| [`a82144d2a9`](https://github.com/qilingframework/qiling/commit/a82144d2a929725d98d36a335ff6435fc8d26bfb) | Add stm32f103 DMA interrupt setting | Authored commit |
| [`91ea1078a4`](https://github.com/qilingframework/qiling/commit/91ea1078a431ccc11016fa6b6ee7a73e18161df8) | Uncompress adio register | Authored commit |
| [`59b90d3aae`](https://github.com/qilingframework/qiling/commit/59b90d3aae754ba70d23c12ea39ce0641aef4452) | Delete stm32f4 dma magic number | Authored commit |
| [`b92e75ea9a`](https://github.com/qilingframework/qiling/commit/b92e75ea9a3d5d1081552ef9106c925303fc58f3) | Fix RCC const typo | Authored commit |
| [`3c7245b070`](https://github.com/qilingframework/qiling/commit/3c7245b07037cd664eb03c77c45ced2f8c44701b) | Fix RCC const name | Authored commit |
| [`89fddb57d4`](https://github.com/qilingframework/qiling/commit/89fddb57d477b5ab55b22e2cb29f1918c3f6f65a) | Add stm32f1xx afio | Authored commit |
| [`9c58c8c340`](https://github.com/qilingframework/qiling/commit/9c58c8c340c96f80cb15a643a7bb8b6916189ebd) | Add stm32f1xx gpio | Authored commit |
| [`1c77daa431`](https://github.com/qilingframework/qiling/commit/1c77daa431bd6e39476dee39e5538dbff8f0cede) | Add stm32f1xx exti | Authored commit |
| [`c46314f99c`](https://github.com/qilingframework/qiling/commit/c46314f99cc3003c1c1342b54b5fa53c9468b2cc) | Add stm32f1xx flash | Authored commit |
| [`4133f7e7d3`](https://github.com/qilingframework/qiling/commit/4133f7e7d3ad2c84f7208d65c82cdb13dc416a9c) | Add stm32f1 usart | Authored commit |
| [`6331207af7`](https://github.com/qilingframework/qiling/commit/6331207af747073a766e283de2514744fda81a5a) | Add stm32f1xx RCC | Authored commit |
| [`1c831e540d`](https://github.com/qilingframework/qiling/commit/1c831e540db47df6c5a5884df74b61edd8869702) | Summary stm32 RCC | Authored commit |
| [`5e998be73f`](https://github.com/qilingframework/qiling/commit/5e998be73f2c7c1d8201b4306ae19c47bb789780) | Replace class with struct | Authored commit |
| [`971d7aabcf`](https://github.com/qilingframework/qiling/commit/971d7aabcf0d56b1c7ba8bf9105d00c41d6c5cf6) | Add cortex series SCB | Authored commit |
| [`43094aeeb9`](https://github.com/qilingframework/qiling/commit/43094aeeb9d611d0fc1b41afb3573fd4496ebfa7) | Fix the format cm4 | Authored commit |
| [`9b13199d47`](https://github.com/qilingframework/qiling/commit/9b13199d47775ee36cbd6aa3cd4e5020d75d10cd) | Add Cortex M3 NVIC | Authored commit |
| [`b342d9b1c9`](https://github.com/qilingframework/qiling/commit/b342d9b1c995d57fb2b5f6563580af859369084d) | Delete rebundant import | Authored commit |
| [`f3886f1d75`](https://github.com/qilingframework/qiling/commit/f3886f1d75ad44e3f3bc0fe68d93f4c77e18dc43) | Add CortexM3 Timer | Authored commit |
| [`df9a1de3ac`](https://github.com/qilingframework/qiling/commit/df9a1de3acb3f796846985c903b8aea2bbc44b75) | Add stm32f103 support | Authored commit |
| [`d4184a49a8`](https://github.com/qilingframework/qiling/commit/d4184a49a8af185f71b74cf4da32d22e5a038d99) | Make stm32f103 config | Authored commit |
| [`ea92ed9c4a`](https://github.com/qilingframework/qiling/commit/ea92ed9c4abd7c513c5da56a9d2fbe7a750b82e7) | Format GD32 config format | Authored commit |
| [`e5d6c4059d`](https://github.com/qilingframework/qiling/commit/e5d6c4059dba5deb00ff6fd998a3a6768c86cb8c) | Simplify arch peripheral name | Authored commit |
| [`3421233afb`](https://github.com/qilingframework/qiling/commit/3421233afbe237d71a835f28f83c5e47c6ceb164) | Format stm32f4 config | Authored commit |
| [`ff0efbdd0c`](https://github.com/qilingframework/qiling/commit/ff0efbdd0cffbbb5203fb2d58aa552d730f75182) | Add BES2300 config | Authored commit |
| [`bc480758da`](https://github.com/qilingframework/qiling/commit/bc480758dafe36c7158d19b3f7dcef01f33f304b) | Merge branch 'dev' into stm32f4 | Authored commit |
| [`4a0dfae32a`](https://github.com/qilingframework/qiling/commit/4a0dfae32a8efdf2379c37aecfbc5b1cb3392f68) | Handle the remap option | Authored commit |
| [`712a79e99a`](https://github.com/qilingframework/qiling/commit/712a79e99a2928fec7ba26a22e38417732aa5938) | Add "remap" item in stm32 config | Authored commit |
| [`2ceb6c5b6f`](https://github.com/qilingframework/qiling/commit/2ceb6c5b6f4c4add2b0fca9d59f14a7a0168331e) | Add pc to the peripheral monitor output | Authored commit |
| [`87ccbcca09`](https://github.com/qilingframework/qiling/commit/87ccbcca095b4179ef8e980ef087ad4314c1f360) | Add sdio intno default value | Authored commit |
| [`4532639001`](https://github.com/qilingframework/qiling/commit/4532639001c9fc4b00aa5e7e881ae7710bb04b44) | Add intno class | Authored commit |
| [`77fd958188`](https://github.com/qilingframework/qiling/commit/77fd95818859626bc23a7099469cef76d5736ab5) | Add SD Card class | Authored commit |
| [`2bd1a1d01d`](https://github.com/qilingframework/qiling/commit/2bd1a1d01d5d5dcbf037db7446d42ac048e5962c) | Add stm32f4xx sdio class | Authored commit |
| [`5c99af9201`](https://github.com/qilingframework/qiling/commit/5c99af9201e914b5243369835951f03114e05ea0) | Fix the interrupt details | Authored commit |
| [`87238d88d9`](https://github.com/qilingframework/qiling/commit/87238d88d9089ae9a4b2cdf18b1f59870bc10505) | Handle all possibile unicorn exception | Authored commit |
| [`3956465758`](https://github.com/qilingframework/qiling/commit/39564657581b9a175253f3d2edaecead6ec571ae) | Fix the nonstop bug | Authored commit |
| [`e2627e2817`](https://github.com/qilingframework/qiling/commit/e2627e2817a1823adeef605c7fe2e561fe5d57e6) | Merge branch 'dev' into stm32f4 | Authored commit |
| [`cd26a68dff`](https://github.com/qilingframework/qiling/commit/cd26a68dff18aa4625c95eb6f7579b28dfe9967c) | Add mnist examples | Authored commit |
| [`3b8197429c`](https://github.com/qilingframework/qiling/commit/3b8197429cd58b2f83c5ebceea4d1cd6b3193a34) | Rename ai test to gpio hook examples | Authored commit |
| [`2120d0f763`](https://github.com/qilingframework/qiling/commit/2120d0f76356981823ca8225535479e825c5047e) | Add header in example | Authored commit |
| [`aac25da360`](https://github.com/qilingframework/qiling/commit/aac25da3606da0cea889c266759cf209063e216b) | Delete useless import | Authored commit |
| [`75c84e1ed2`](https://github.com/qilingframework/qiling/commit/75c84e1ed2e56c4b9336a7ed92f832d5b3b3f018) | Add a ML and oled example | Authored commit |
| [`c45a0e66af`](https://github.com/qilingframework/qiling/commit/c45a0e66af124ae03906fe5aaa82fe3b3edff2ea) | Add stm32f407 CRC examples | Authored commit |
| [`6e34554375`](https://github.com/qilingframework/qiling/commit/6e34554375ce4ebc3824338106d099e22c068394) | Update the hook_set/reset api | Authored commit |
| [`f59bff854d`](https://github.com/qilingframework/qiling/commit/f59bff854d35d87708d59b7f31623e9ccb62c50b) | Refactor the gpio hook | Authored commit |
| [`e010183bb3`](https://github.com/qilingframework/qiling/commit/e010183bb35baaa3ada8944a3ff61563dbde97e9) | Add CRC Support | Authored commit |
| [`747413c710`](https://github.com/qilingframework/qiling/commit/747413c710235f338ba98c1410a8dfaa91ddbf58) | Add stn32 DBG struct | Authored commit |
| [`c6f72c72d7`](https://github.com/qilingframework/qiling/commit/c6f72c72d7542f302476cd7757190eb0fda2582d) | Add device id in dbgmcu and fix critical typo | Authored commit |
| [`44d4c355bb`](https://github.com/qilingframework/qiling/commit/44d4c355bb302ef9ea570ef914354729de98b00a) | elong the ppb segment | Authored commit |
| [`2892ef323b`](https://github.com/qilingframework/qiling/commit/2892ef323bd73f4ec833aa39f1f00af96337f4f0) | Merge branch 'dev' into stm32f4 | Authored commit |
| [`7a2b5badc2`](https://github.com/qilingframework/qiling/commit/7a2b5badc2e540995b4f431e7460dfd2c1ffa318) | Add 'Flash Interface' into stm32f4 config | Authored commit |
| [`7dae9f4e69`](https://github.com/qilingframework/qiling/commit/7dae9f4e69577c63f9319bec2f53381d4da25afa) | Delete a dup typo of DAC | Authored commit |
| [`35f0e7117b`](https://github.com/qilingframework/qiling/commit/35f0e7117b83b51716e30a2fbfc420d0337304be) | Update rootfs | Authored commit |
| [`0799734fb8`](https://github.com/qilingframework/qiling/commit/0799734fb8ef55fcf9e7814aac78d34ca302c524) | Merge branch 'dev' into stm32f4 | Authored commit |
| [`6a917ffc98`](https://github.com/qilingframework/qiling/commit/6a917ffc98211352c91dc3ce8a2f7c776900f69d) | Add spi oled examples | Authored commit |
| [`6337caa09e`](https://github.com/qilingframework/qiling/commit/6337caa09e9ee2719b4594335a53bf8105b3429e) | Delete the debug print | Authored commit |
| [`a284b75669`](https://github.com/qilingframework/qiling/commit/a284b75669f39d7df5f1d79dad1ad077a8d2892c) | Add SSD1306 (OLED12864) render | Authored commit |
| [`8841f75a8e`](https://github.com/qilingframework/qiling/commit/8841f75a8ecf9ef3f3768d1dff59f9dbb6ec0673) | Add OLED folder | Authored commit |
| [`78918cb939`](https://github.com/qilingframework/qiling/commit/78918cb9393d2c88490f905ab11bb1a86f1e7bd4) | Fix lcd class name | Authored commit |
| [`b92729efa7`](https://github.com/qilingframework/qiling/commit/b92729efa785b6f560e7958e0931658cad795227) | Revert the freertos test | Authored commit |
| [`5b3dc7e1f6`](https://github.com/qilingframework/qiling/commit/5b3dc7e1f6b1870953e785efdb55950fc70b322b) | Throw warning in default | Authored commit |
| [`c5e68f7e89`](https://github.com/qilingframework/qiling/commit/c5e68f7e89fcf60679d25c27ddf178e7ba08dcdc) | Patch flash and pwr read and write | Authored commit |
| [`55c3136fc3`](https://github.com/qilingframework/qiling/commit/55c3136fc30bc216e8b80a216ed3ebe9a3a596bd) | Merge branch 'dev' into stm32f4 | Authored commit |
| [`4a7baa58e9`](https://github.com/qilingframework/qiling/commit/4a7baa58e9ccb965c1503f230457897e92970e8f) | Add STM32 TIM test | Authored commit |
| [`4859ef1fa3`](https://github.com/qilingframework/qiling/commit/4859ef1fa3fdfd6b75835f2d7d2b14735735aee9) | Fix reset bug | Authored commit |
| [`e43f7cb429`](https://github.com/qilingframework/qiling/commit/e43f7cb429ca4e306a4233e39a5326fb504a2219) | Add update interrupt and count down in TIM1 | Authored commit |
| [`5bbf584cbf`](https://github.com/qilingframework/qiling/commit/5bbf584cbf2e7f0ede99f8ea1d891a7b828c99f8) | Use timer base class in systick | Authored commit |
| [`4efac22082`](https://github.com/qilingframework/qiling/commit/4efac22082280ab53dbd4dbb6817833393ba7012) | Add abstract timer class | Authored commit |
| [`579a5d992e`](https://github.com/qilingframework/qiling/commit/579a5d992e19020593048ad38cf3a798fc8875bb) | Add Timer const file | Authored commit |
| [`4ac1d5c862`](https://github.com/qilingframework/qiling/commit/4ac1d5c8621dae05bfd5987f9c6d2f7bbf162537) | Rename gd32 const files | Authored commit |
| [`00cf83f45b`](https://github.com/qilingframework/qiling/commit/00cf83f45bbfcef0a4a153a24ea90796c6e0ce5a) | Update latest rootfs | Authored commit |
| [`852475b1fb`](https://github.com/qilingframework/qiling/commit/852475b1fb847d7ce824f9abd8898cfe9a6e4446) | Merge branch 'dev' into stm32f4 | Authored commit |
| [`c9de30c886`](https://github.com/qilingframework/qiling/commit/c9de30c8861dcb9387c0b08d29d22ec2de0da59b) | Add basic TIM struct | Authored commit |
| [`d5dee1f9da`](https://github.com/qilingframework/qiling/commit/d5dee1f9da2b450599efa6f4692c851af37497d7) | Add flash interface struct | Authored commit |
| [`536834595e`](https://github.com/qilingframework/qiling/commit/536834595e5cf5f71aa7946effaf75e926a99c52) | Add flash interface in config | Authored commit |
| [`4f10394e88`](https://github.com/qilingframework/qiling/commit/4f10394e8819ed7ebfa5470910856a5e7d5acef2) | Format the RCC rdyon code | Authored commit |
| [`24d8f368da`](https://github.com/qilingframework/qiling/commit/24d8f368da0a072a1ac64efb877a8a17453491fb) | Add header for mcu examples | Authored commit |
| [`803cc387f5`](https://github.com/qilingframework/qiling/commit/803cc387f5e10c2444457c2fa4b1c5b826ac362f) | Add I2C Interrupt into examples | Authored commit |
| [`d3f28a747a`](https://github.com/qilingframework/qiling/commit/d3f28a747a7c88745bef7fff84ecbf62b7c9ba7b) | Add I2C Interrupt testcase | Authored commit |
| [`34958ed482`](https://github.com/qilingframework/qiling/commit/34958ed48282d39c2f6e4e8afc614b1068dd0b90) | Pass the i2c interrupt case | Authored commit |
| [`1162e26295`](https://github.com/qilingframework/qiling/commit/1162e26295f3a8b6a3b61420f1f418949096786e) | Add recorder for i2c | Authored commit |
| [`f509bba6d8`](https://github.com/qilingframework/qiling/commit/f509bba6d81ef39bbbf86f11ea956ab58e434ab9) | Add peripheral recorder | Authored commit |
| [`8abc8cbf19`](https://github.com/qilingframework/qiling/commit/8abc8cbf19064b306dd889a0e3e0e359ca3c7c49) | Add access recorder | Authored commit |
| [`5f738c842f`](https://github.com/qilingframework/qiling/commit/5f738c842f4a9e4e9405d086d4cbdeeea6eaafcf) | Enable monitor in default | Authored commit |
| [`8003f6cdd0`](https://github.com/qilingframework/qiling/commit/8003f6cdd092f1da3b44a8e271746ab7f1fce993) | Change peripheral decorator name | Authored commit |
| [`1e89e144e6`](https://github.com/qilingframework/qiling/commit/1e89e144e670ec8ec02af5a854f8935a01044d50) | Change peripheral monitor log level | Authored commit |
| [`ec456db61e`](https://github.com/qilingframework/qiling/commit/ec456db61ef6c838c2661589a181835beea473e9) | Fix a mcu elf loader bug | Authored commit |
| [`88fb9390f7`](https://github.com/qilingframework/qiling/commit/88fb9390f7ac4d4d2130729bfe1681eb69a875aa) | Fix mcu test (soc -> mcu) | Authored commit |
| [`2e87790ef5`](https://github.com/qilingframework/qiling/commit/2e87790ef5818a8955f0bbd401c72ca446939cfd) | Fix ext (soc -> mcu) | Authored commit |
| [`14b95eb94a`](https://github.com/qilingframework/qiling/commit/14b95eb94a2ec174a36da904d1f2bfe91f47959a) | Fix examples (soc -> mcu) | Authored commit |
| [`b543f0dc4a`](https://github.com/qilingframework/qiling/commit/b543f0dc4aa7edd87b1a5c53563bc2ae016af63c) | Fix the mcu test | Authored commit |
| [`f8db1fe828`](https://github.com/qilingframework/qiling/commit/f8db1fe828bb086b5d0551f1c7666d800915a895) | Cut env suffix | Authored commit |
| [`baf04bc135`](https://github.com/qilingframework/qiling/commit/baf04bc1356176ecfe23bc6814a5c9aeed64d966) | Fix the examples | Authored commit |
| [`915969800d`](https://github.com/qilingframework/qiling/commit/915969800d5afe0abcea727af526e8150ed81693) | Cut 'env' suffix | Authored commit |
| [`b68b8dae58`](https://github.com/qilingframework/qiling/commit/b68b8dae588f446295510c8c14e15270991c4635) | Avoid the capstone error | Authored commit |
| [`d98f25840e`](https://github.com/qilingframework/qiling/commit/d98f25840e9967481c0f5866e0070d30df79a8a5) | Merge branch 'dev' into gd32 | Authored commit |
| [`5ff427f156`](https://github.com/qilingframework/qiling/commit/5ff427f1564f5aa038ac89387819855f172cee2a) | Add yaml in requirement | Authored commit |
| [`da4624f659`](https://github.com/qilingframework/qiling/commit/da4624f6593e8b6bb7d3a731c63f80072e85d3c7) | Add test profiles | Authored commit |
| [`4d042f3fd7`](https://github.com/qilingframework/qiling/commit/4d042f3fd7ee56f78f129ebfe32fbdbbda544fcd) | Test covered profile in MCU | Authored commit |
| [`56522c5e9a`](https://github.com/qilingframework/qiling/commit/56522c5e9a2b757db6e9833a0cd363399b2309ec) | Cover env by profile | Authored commit |
| [`ec285ac61a`](https://github.com/qilingframework/qiling/commit/ec285ac61ac6e011c06f0304ae611346116e64e5) | load baremetal profile by yaml | Authored commit |
| [`816bf9612a`](https://github.com/qilingframework/qiling/commit/816bf9612a8765fbcb7ac2e715febd832407b28b) | Delete baremetal profile setup | Authored commit |
| [`2b055ed9ef`](https://github.com/qilingframework/qiling/commit/2b055ed9ef0070dd13109add0f82cacabc4df7f3) | Add banner in hw.utils files | Authored commit |
| [`233e997e29`](https://github.com/qilingframework/qiling/commit/233e997e29057f9589d33c67f0331252753944d4) | Add banner in hw.timer files | Authored commit |
| [`86edea1edf`](https://github.com/qilingframework/qiling/commit/86edea1edf86785a92a513d5dcf25d039e18a62c) | Add banner in hw.spi files | Authored commit |
| [`3f8cdc1694`](https://github.com/qilingframework/qiling/commit/3f8cdc1694c5660aa83ff4016be36366e421a9e1) | Add banner in hw.power files | Authored commit |
| [`aefb0a82c7`](https://github.com/qilingframework/qiling/commit/aefb0a82c788637dd609c073db2ffdfeed354a1f) | Add banner in hw.misc files | Authored commit |
| [`90047f7379`](https://github.com/qilingframework/qiling/commit/90047f737954992b25718a4f83d27e1025ed8c45) | Add banner in hw.math files | Authored commit |
| [`3887a717f1`](https://github.com/qilingframework/qiling/commit/3887a717f181886ff5c98a13170be4e4031baec3) | Add banner in hw.intc files | Authored commit |
| [`ce895a980e`](https://github.com/qilingframework/qiling/commit/ce895a980eeaf2ecc0f555b1f65c4a5b3bc7ae85) | Add banner in hw.i2c files | Authored commit |
| [`f34ec0c637`](https://github.com/qilingframework/qiling/commit/f34ec0c6379df426992b0441fd80e1e348d0f5fe) | Add banner in hw.gpio files | Authored commit |
| [`feedf7b22d`](https://github.com/qilingframework/qiling/commit/feedf7b22d2f89c348b3ffc25b22481ce8913903) | Add banner in __init__ files | Authored commit |
| [`09634ece7f`](https://github.com/qilingframework/qiling/commit/09634ece7f089097f51efa44a9fd7f9a5b49972c) | Add banner in hw.dma files | Authored commit |
| [`a41c24b3b6`](https://github.com/qilingframework/qiling/commit/a41c24b3b65e3adc024fcf4cba714c33179c45b7) | Add banner in hw const files | Authored commit |
| [`ec754f943f`](https://github.com/qilingframework/qiling/commit/ec754f943f9d754b262d7a8482591cf56418c6b1) | Add banner in char device files | Authored commit |
| [`7271387a26`](https://github.com/qilingframework/qiling/commit/7271387a26480b76f82fbf7889721a6ab9c263e9) | Delete outdate profiles | Authored commit |
| [`0195e3daba`](https://github.com/qilingframework/qiling/commit/0195e3dabae3b157c9341674b4355ba56dd30479) | Fix test_mcu | Authored commit |
| [`dedb09db1d`](https://github.com/qilingframework/qiling/commit/dedb09db1debc5cffdbfd210249d0d2c9df824b2) | Replace profile with env in mcu | Authored commit |
| [`92b0a3dd8a`](https://github.com/qilingframework/qiling/commit/92b0a3dd8addd197deec66f38d2d6e7f723a2043) | Add gd32vf103 env | Authored commit |
| [`6d3b2d1527`](https://github.com/qilingframework/qiling/commit/6d3b2d1527e174e84a80ef661d31f09d8ad28a18) | Replace profile with env in hw | Authored commit |
| [`161b200c93`](https://github.com/qilingframework/qiling/commit/161b200c93cf6d6958f9c856809a2201dcd17642) | Fix the gd32vf103_blink example | Authored commit |
| [`95a9ccb9cf`](https://github.com/qilingframework/qiling/commit/95a9ccb9cf74d29c620786208770b0cc9bce67c1) | Fix stm32f411_i2c_lcd example | Authored commit |
| [`a0fff057b9`](https://github.com/qilingframework/qiling/commit/a0fff057b92a58aa305f97552225bb778130c834) | Fix stm32f411_interact_usart example | Authored commit |
| [`f63968a776`](https://github.com/qilingframework/qiling/commit/f63968a77622cfb5882dac0dc6e56c3792058826) | Fix stm32f411_freertos example | Authored commit |
| [`75b63546cb`](https://github.com/qilingframework/qiling/commit/75b63546cb5eedd1bd6287ff485e15cbe236e749) | Fix stm32f411_dma_logger examples | Authored commit |
| [`2a3a47244e`](https://github.com/qilingframework/qiling/commit/2a3a47244ea49a6e4a8e436e8ba9b7e7355a164d) | Fix the stm32f407 example | Authored commit |
| [`4c67418347`](https://github.com/qilingframework/qiling/commit/4c6741834777b751073a63eaed8b90a8dda31c7d) | Fix the 'stm32f411_gpio_hook' example | Authored commit |
| [`bf95975d64`](https://github.com/qilingframework/qiling/commit/bf95975d64ecf005a1da452b2e41a7f25183e788) | Convert profile into env | Authored commit |
| [`9b3b1caa4a`](https://github.com/qilingframework/qiling/commit/9b3b1caa4a8ba6f3f7cb4752a3093dac5b0a3589) | Merge branch 'dev' into gd32 | Authored commit |
| [`a6f91e2162`](https://github.com/qilingframework/qiling/commit/a6f91e21627c4986efcff709e7c2690f6fea258b) | Update the warning output | Authored commit |
| [`d8abe2544b`](https://github.com/qilingframework/qiling/commit/d8abe2544bdcc1c60671b0eca94e532b94b24b57) | Add GD32 hello world example | Authored commit |
| [`9f1e3afcd6`](https://github.com/qilingframework/qiling/commit/9f1e3afcd6eb001b7430cae7b9b5563e1535d20d) | Add GD32 led test | Authored commit |
| [`91eb5ee9b9`](https://github.com/qilingframework/qiling/commit/91eb5ee9b9a937e10883251be66094481e07e3c9) | Add gd32 gpio logic | Authored commit |
| [`a78ca6c756`](https://github.com/qilingframework/qiling/commit/a78ca6c756c2a04a4e9cc6ef385d6434b240af85) | Add monitor to eclic | Authored commit |
| [`1aecf6e81b`](https://github.com/qilingframework/qiling/commit/1aecf6e81b45f4ab8d156ebc1d6a42996a95020d) | Fix the argument typo | Authored commit |
| [`d1cb342c0e`](https://github.com/qilingframework/qiling/commit/d1cb342c0eb4bb65948857b0a4ae8a661cea3737) | Fix the "peripheral" typo | Authored commit |
| [`1b036835ae`](https://github.com/qilingframework/qiling/commit/1b036835aea501f8783da46bd73dc95cca9505d7) | Update the profile of gd32vf103 | Authored commit |
| [`c1c85534f3`](https://github.com/qilingframework/qiling/commit/c1c85534f3aafcb5e3c626f77265e12392183984) | Add monitor to gd32rcu | Authored commit |
| [`5b98d7fa63`](https://github.com/qilingframework/qiling/commit/5b98d7fa6338617adcfd2276bc8fcda9d43b5b69) | Add monitor to gd32gpio | Authored commit |
| [`b309c84f1e`](https://github.com/qilingframework/qiling/commit/b309c84f1e8e2d5c30f029c459b9b2a4ef5983a7) | Delete self.path | Authored commit |
| [`d4b1907207`](https://github.com/qilingframework/qiling/commit/d4b19072074f4e21ce89bd2edcd46f07efa75253) | Simplify mcu loader code | Authored commit |
| [`81b39ea99c`](https://github.com/qilingframework/qiling/commit/81b39ea99c0cc9525b85df91ea72f78f972fbbaf) | Merge branch 'gd32' of https://github.com/cla7aye15I4nd/qiling into gd32 | Authored commit |
| [`f6010237a6`](https://github.com/qilingframework/qiling/commit/f6010237a6d4ce888783e21aaf06fc00e91c23c9) | Update api name | Authored commit |
| [`0bf1060e86`](https://github.com/qilingframework/qiling/commit/0bf1060e869f001f55c10d6b3da29b956b39cabc) | Add basic function for running | Authored commit |
| [`a4e7357703`](https://github.com/qilingframework/qiling/commit/a4e73577031cdfb860d84b7b51af677a91739da1) | Update both 32 and 64 bit statx | Authored commit |
| [`94df6e8aad`](https://github.com/qilingframework/qiling/commit/94df6e8aad064ea8c62cc0388b4af8c41f9577a0) | Add some comment for statx | Authored commit |
| [`0afd7580eb`](https://github.com/qilingframework/qiling/commit/0afd7580eb4456bb4621ecfc1baa343b255d9243) | Add riscv32 dynamic testcase | Authored commit |
| [`9d3f55e6e6`](https://github.com/qilingframework/qiling/commit/9d3f55e6e64c037ec9793c085714eae8c5a5e635) | patch elf parser | Authored commit |
| [`7325612a4d`](https://github.com/qilingframework/qiling/commit/7325612a4df6340db2f2325610e905bf3c6e222b) | Fix the stat structure | Authored commit |
| [`d2a44a18ce`](https://github.com/qilingframework/qiling/commit/d2a44a18ce8b86ed13ec160b9c36a92a3c2f46e6) | Fix the riscv32 syscall table | Authored commit |
| [`7b6d3a82f4`](https://github.com/qilingframework/qiling/commit/7b6d3a82f495440e665a47859e8bc8b5068c93e0) | Add statx syscall | Authored commit |
| [`897d28f655`](https://github.com/qilingframework/qiling/commit/897d28f655bc4a79596e4fe4dc14b304a596d9e6) | Simplify the openat dirfd handle method | Authored commit |
| [`df5bdf0460`](https://github.com/qilingframework/qiling/commit/df5bdf0460422dcbe54153457f84d0a1134671bf) | Update the openat syscall | Authored commit |
| [`94a950cc55`](https://github.com/qilingframework/qiling/commit/94a950cc55776395d2a9a5e5c499a05d8ae18d6c) | Update AT_FDCWD const | Authored commit |
| [`9a166b35f4`](https://github.com/qilingframework/qiling/commit/9a166b35f4808d7658cc9445ed64e00606d65a42) | Merge branch 'dev' into riscv | Authored commit |
| [`c2e17a4222`](https://github.com/qilingframework/qiling/commit/c2e17a4222fd7bf555e422c52382941e67708791) | Fix core typo | Authored commit |
| [`f8a2578945`](https://github.com/qilingframework/qiling/commit/f8a2578945ef8d7c64bd0810a4b60899cbd0fd93) | Test the riscv mcu setup | Authored commit |
| [`4b115ed187`](https://github.com/qilingframework/qiling/commit/4b115ed18782ba2de8ada0d8b08e49cc87605d2e) | Add reset_register api | Authored commit |
| [`9f2244cf8c`](https://github.com/qilingframework/qiling/commit/9f2244cf8c9c4a2faf57a01c184151bf10991fce) | Split loader and arch | Authored commit |
| [`9f653f0de1`](https://github.com/qilingframework/qiling/commit/9f653f0de1c68ca6c934f8c44caffe391d2f5a33) | Rename the interrupt handler | Authored commit |
| [`fc2edaa10f`](https://github.com/qilingframework/qiling/commit/fc2edaa10fa3fcc0b69964942d171bff34245f36) | Merge branch 'gd32' into riscv | Authored commit |
| [`9abeaaff16`](https://github.com/qilingframework/qiling/commit/9abeaaff167fa741fade3ef46b8b1e7258080819) | Add intr_handler API | Authored commit |
| [`6e25dc2f9b`](https://github.com/qilingframework/qiling/commit/6e25dc2f9ba32b70c860f6daa8e009e8b08fadce) | Merge branch 'dev' into riscv | Authored commit |
| [`15185cbf53`](https://github.com/qilingframework/qiling/commit/15185cbf53ad5e3bc9345e863379bc760ea353eb) | Refactor the core setup workflow | Authored commit |
| [`28e7e47190`](https://github.com/qilingframework/qiling/commit/28e7e47190e9cf8f1ee235944168d748b910b499) | Remove evm file mode temporary | Authored commit |
| [`e6d0a9b38a`](https://github.com/qilingframework/qiling/commit/e6d0a9b38a84d3e5b9fdcde21b809e212ac02884) | Add alias map for arch/os convert function | Authored commit |
| [`8a0b14c747`](https://github.com/qilingframework/qiling/commit/8a0b14c7477b4c1de62db7fc1dfbe5e696f9ae72) | Refactor the core const mapping | Authored commit |
| [`3fc8b7f038`](https://github.com/qilingframework/qiling/commit/3fc8b7f03862d79cce05cb0a307d93f7066175e4) | Add gd32 config | Authored commit |
| [`80f9dac85d`](https://github.com/qilingframework/qiling/commit/80f9dac85d023e64e1b240a785eb91c2a60605ac) | Fix the `mknodat` path argument | Authored commit |
| [`94c394e5ed`](https://github.com/qilingframework/qiling/commit/94c394e5ed4da9e46107e2fc244ecef759f13f80) | Fix the wrong import | Authored commit |
| [`b9fd571f73`](https://github.com/qilingframework/qiling/commit/b9fd571f73471cf137d2bb6563f4ce16c4faef46) | Merge branch 'riscv' of https://github.com/cla7aye15I4nd/qiling into riscv | Authored commit |
| [`7dc0d6b220`](https://github.com/qilingframework/qiling/commit/7dc0d6b220ec1b27d3c798d89f90894a8bcd0001) | Fix the dirfd argument | Authored commit |
| [`613ae212ba`](https://github.com/qilingframework/qiling/commit/613ae212baabd9616fb7b518abde34e5398e2a46) | Add AT_FDCWD const | Authored commit |
| [`32ff7d027e`](https://github.com/qilingframework/qiling/commit/32ff7d027e9b143885d396185e5ad3cf9102dd90) | Merge branch 'dev' into riscv | Authored commit |
| [`025cfc304e`](https://github.com/qilingframework/qiling/commit/025cfc304e9ca0b9004a166717c33bf8c57d154f) | Fix wrong space | Authored commit |
| [`cbcbf9cd4e`](https://github.com/qilingframework/qiling/commit/cbcbf9cd4e69a7118c702cbdc6c2f3e2fb44eef8) | Add defualt float support | Authored commit |
| [`ec3494899d`](https://github.com/qilingframework/qiling/commit/ec3494899d2651984797de5733696ef79697bc69) | Update the register map to rc4 | Authored commit |
| [`0ec3783e57`](https://github.com/qilingframework/qiling/commit/0ec3783e57fc0ad1108f03eb816b50a026fb43e3) | Fix the riscv test | Authored commit |
| [`6e2213ef00`](https://github.com/qilingframework/qiling/commit/6e2213ef007aa5f31b717544fff11eacc5f823fc) | Refactor the output of syscall | Authored commit |
| [`c67c5388ad`](https://github.com/qilingframework/qiling/commit/c67c5388ad2d53aa7dff0bb08975c030ad361df4) | Add LinuxRISCVStat | Authored commit |
| [`208edddacf`](https://github.com/qilingframework/qiling/commit/208edddacf3a537e7fc0c53ed179b2c3d5203126) | Add riscv dyn testcase | Authored commit |
| [`baa86ab6a4`](https://github.com/qilingframework/qiling/commit/baa86ab6a4d1a954671290acdd22fd8caa7d3979) | Fix some typo | Authored commit |
| [`f524ab1c85`](https://github.com/qilingframework/qiling/commit/f524ab1c857954223cf54b9cbb8d5c9554f6f385) | Warning is ok when intrrupt | Authored commit |
| [`937a594fe1`](https://github.com/qilingframework/qiling/commit/937a594fe1d06a38984ecd759660b696b8535138) | Refactor the mman | Authored commit |
| [`045f97cf25`](https://github.com/qilingframework/qiling/commit/045f97cf25739e8fd47a86fc88525704deff5ab9) | Add riscv linux open flags | Authored commit |
| [`3786178236`](https://github.com/qilingframework/qiling/commit/3786178236a6edc4c13d79bef9d99f0b9d69d0dd) | Fix riscv function hook | Authored commit |
| [`9b650c05d5`](https://github.com/qilingframework/qiling/commit/9b650c05d51e1d5b96a8fcfcab95f9c6e4870997) | Avoid close stdout during test | Authored commit |
| [`a181d00c3e`](https://github.com/qilingframework/qiling/commit/a181d00c3e782fa6ad4a439727d0f9fe927012c7) | Append riscv testcase | Authored commit |
| [`b5804b726d`](https://github.com/qilingframework/qiling/commit/b5804b726da16f07095628e229d8163e078333b5) | Try update the unicorn version | Authored commit |
| [`45dd725ff5`](https://github.com/qilingframework/qiling/commit/45dd725ff53fbe4265011835e83a704c3fd0233a) | Update the riscv32 syscall table | Authored commit |
| [`d2bad75b2a`](https://github.com/qilingframework/qiling/commit/d2bad75b2ab31fd7a4da929695c28abf6edddf4d) | Merge branch 'dev' into riscv | Authored commit |
| [`d1db42ebf3`](https://github.com/qilingframework/qiling/commit/d1db42ebf32f118c69c680628984d78d558e3dfd) | Merge pull request #985 from cla7aye15I4nd/dev | Authored commit |
| [`57807a52fd`](https://github.com/qilingframework/qiling/commit/57807a52fd01f411bad4fc71a46c47e9c8c14a95) | Merge branch 'dev' of https://github.com/cla7aye15I4nd/qiling into dev | Authored commit |
| [`4fa58f219e`](https://github.com/qilingframework/qiling/commit/4fa58f219e672c90974ef08623052a3aff717785) | Add gd32 const files | Authored commit |
| [`b19c313a10`](https://github.com/qilingframework/qiling/commit/b19c313a1062d8d611cb4e87f3df8179319c0a65) | Add gd32 spi component | Authored commit |
| [`d517e94e19`](https://github.com/qilingframework/qiling/commit/d517e94e1933d142404d56ef772d570f861bdd91) | Add gd32 i2c component | Authored commit |
| [`aed1cf2cd7`](https://github.com/qilingframework/qiling/commit/aed1cf2cd75cdf16d8ef5eb0396525eae767f3af) | Add GD32 DMA component | Authored commit |
| [`78687ce4f3`](https://github.com/qilingframework/qiling/commit/78687ce4f363c916245171d0877ed6498e5dd9cf) | Add gd32 interrupt controller | Authored commit |
| [`cc1c3bdc5d`](https://github.com/qilingframework/qiling/commit/cc1c3bdc5da3de7f9b6d63297ec510ad366bbdd4) | Add GD32 crc component | Authored commit |
| [`e359dfa7d8`](https://github.com/qilingframework/qiling/commit/e359dfa7d8966dc970a3b99a1131ba88a3c694db) | Add gd32 rtc and timer component | Authored commit |
| [`a0bb91b57a`](https://github.com/qilingframework/qiling/commit/a0bb91b57a2899cfcbae4004bf689b136c6b7396) | Add gd32 rcu component | Authored commit |
| [`3732dea9fd`](https://github.com/qilingframework/qiling/commit/3732dea9fdfd6708200b3c478890c255bb1ab930) | Add GD32 GPIO component | Authored commit |
| [`34d0700f3b`](https://github.com/qilingframework/qiling/commit/34d0700f3b2d61e069abfcd45c1299b4b3cf35ba) | Add GD32 usart component | Authored commit |
| [`4e3d5d3a97`](https://github.com/qilingframework/qiling/commit/4e3d5d3a97710f068a6a9ea8cb1dd4142de7b744) | Merge pull request #981 from cla7aye15I4nd/dev | Authored commit |
| [`873544c418`](https://github.com/qilingframework/qiling/commit/873544c418210ed9d5f8c57027a4c8a1820faa5f) | Merge branch 'dev' of https://github.com/cla7aye15I4nd/qiling into dev | Authored commit |
| [`8a1ad3ef98`](https://github.com/qilingframework/qiling/commit/8a1ad3ef98992bf6e9b92db33d3cf6562d804e8f) | Replace exception with warning | Authored commit |
| [`96551f603b`](https://github.com/qilingframework/qiling/commit/96551f603b79bbe382dd7f056bc051cbe6d4e255) | Fix the utf-8 decode error | Authored commit |
| [`8699c5239a`](https://github.com/qilingframework/qiling/commit/8699c5239a4473a264bb2b2ff26cfdb8119b651d) | Fix the riscv syscall cc | Authored commit |
| [`619ca43446`](https://github.com/qilingframework/qiling/commit/619ca43446fa7096c0db3d4789ff59c1f344b66d) | Move the riscv cc to new file | Authored commit |
| [`059a47be5b`](https://github.com/qilingframework/qiling/commit/059a47be5b8324a47b7adc2a822d656e86b8aec5) | Fix riscv64 capstone mode | Authored commit |
| [`c910812074`](https://github.com/qilingframework/qiling/commit/c910812074b2c3ff82f18136f7ff925e3cca256a) | Merge branch 'dev' into riscv | Authored commit |
| [`fa42395d15`](https://github.com/qilingframework/qiling/commit/fa42395d150cdeb591ef919472f03d320b4bf5bb) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`ab04e0fe7e`](https://github.com/qilingframework/qiling/commit/ab04e0fe7eec78d5a550c10b9659d8c4e903759d) | Fix the capstone import | Authored commit |
| [`8a514cd3cb`](https://github.com/qilingframework/qiling/commit/8a514cd3cbe6081e07f448569c6535d429422905) | Fix a simple bug in gpio odr | Authored commit |
| [`a6c8d71232`](https://github.com/qilingframework/qiling/commit/a6c8d71232f1e4fd63579b37dcc6c6b183239e80) | Merge pull request #978 from cla7aye15I4nd/dev | Authored commit |
| [`a9a24202c2`](https://github.com/qilingframework/qiling/commit/a9a24202c24242196bf6bb5b8ed78c341ecc180e) | Update qnx syscall table | Authored commit |
| [`0ccf5fc7d3`](https://github.com/qilingframework/qiling/commit/0ccf5fc7d3f874ad04c684e9baafe34408a9341d) | Update macos syscall table | Authored commit |
| [`570a974da7`](https://github.com/qilingframework/qiling/commit/570a974da7ac1abbe86d8afff58b6cdfc76d430b) | Update freebsd syscall table | Authored commit |
| [`d80fcdcedf`](https://github.com/qilingframework/qiling/commit/d80fcdcedfbc8c78f2a65c895e7489b5cfd510cd) | Fix typo in linux map_syscall | Authored commit |
| [`a7ad66f258`](https://github.com/qilingframework/qiling/commit/a7ad66f258499bcd9179044ca2a523f6496ebba6) | Merge pull request #977 from cla7aye15I4nd/dev | Authored commit |
| [`0dbddfed6f`](https://github.com/qilingframework/qiling/commit/0dbddfed6f1ca8eff91eea456aedd4710c1e7fd7) | Add riscv helloworld example source code | Authored commit |
| [`a7baec38be`](https://github.com/qilingframework/qiling/commit/a7baec38be5d43e259b9640e2f1adc256ad1856e) | Enable syscall in riscv | Authored commit |
| [`f75cf9d571`](https://github.com/qilingframework/qiling/commit/f75cf9d5716d3460b4bf04dd6724114029dbd5bf) | Append riscv in arch bit array | Authored commit |
| [`01b2f4658b`](https://github.com/qilingframework/qiling/commit/01b2f4658bedd0d3262de5d4a42080ee07e9177d) | Enable the riscv function hook | Authored commit |
| [`715bf76b4f`](https://github.com/qilingframework/qiling/commit/715bf76b4fe059d2ee2221fdc233cbe324843294) | Add cc for riscv in linux and posix | Authored commit |
| [`1d01267bdf`](https://github.com/qilingframework/qiling/commit/1d01267bdf3721ece371b731e8001b922c94bd9f) | Add elf machine identifier for riscv | Authored commit |
| [`f29b8286aa`](https://github.com/qilingframework/qiling/commit/f29b8286aa7d308f766a9130cfc2db39b810fd31) | Add riscv32/64 arch code | Authored commit |
| [`8372355c45`](https://github.com/qilingframework/qiling/commit/8372355c454b055ed33778683a749ab8bb1128a7) | Add riscv 32/64 bit structure | Authored commit |
| [`59c8803cd8`](https://github.com/qilingframework/qiling/commit/59c8803cd8b8add8025d5fbaa1a3d8cd8791e546) | Add riscv universal register | Authored commit |
| [`fc947cdabf`](https://github.com/qilingframework/qiling/commit/fc947cdabf0cf967899ec32029016251845fbdef) | Remove LCD1602 config file | Authored commit |
| [`852fc4b8ad`](https://github.com/qilingframework/qiling/commit/852fc4b8ad2eff9b948fd6c0ef8f36f00f7cccea) | Optimize the way of finding syscall num | Authored commit |
| [`cc1cb5fb23`](https://github.com/qilingframework/qiling/commit/cc1cb5fb23d405e96ccdb7554fa8279dd4305c2a) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`c5100cb887`](https://github.com/qilingframework/qiling/commit/c5100cb887d84519c66e48062a84b911bad23a81) | Fix the import of cortexm const | Authored commit |
| [`eaf2846f4a`](https://github.com/qilingframework/qiling/commit/eaf2846f4a66389fd78b75e4350b38916e9d58b7) | Create const file for cortexm | Authored commit |
| [`1a1e79c039`](https://github.com/qilingframework/qiling/commit/1a1e79c03985c8d2b309369d4aac9ac493bf779e) | Merge pull request #972 from cla7aye15I4nd/dev | Authored commit |
| [`1180617462`](https://github.com/qilingframework/qiling/commit/1180617462f1b853e15467dae4d8c256c729bec1) | Merge branch 'dev' of https://github.com/cla7aye15I4nd/qiling into dev | Authored commit |
| [`9414ce57c0`](https://github.com/qilingframework/qiling/commit/9414ce57c0b24e4c3bc119e10b71ea840062151a) | Shrink the lcd example again | Authored commit |
| [`69e185eabf`](https://github.com/qilingframework/qiling/commit/69e185eabf11df680ef320ace9027d3e812f3a1e) | Speed up the LCD example | Authored commit |
| [`e5a05e3303`](https://github.com/qilingframework/qiling/commit/e5a05e3303fab2c77969058a679eb58fbd86d65a) | Fix a simple bug in LCD1602 | Authored commit |
| [`54dcf4a27e`](https://github.com/qilingframework/qiling/commit/54dcf4a27ec374a6f722a82b8ed04cdbe936e3df) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`7b8e99f331`](https://github.com/qilingframework/qiling/commit/7b8e99f33110bc66fe8c7219c5d74595b58e227a) | remove the close button | Authored commit |
| [`3cd0bbe3c3`](https://github.com/qilingframework/qiling/commit/3cd0bbe3c3dcde206a4f528f96e7b517963acc1c) | Using new class new | Authored commit |
| [`69f6eded49`](https://github.com/qilingframework/qiling/commit/69f6eded492501999f79f7fabebb5a7a7af7094a) | Add PyGame prefix for class name | Authored commit |
| [`eb2477b0a0`](https://github.com/qilingframework/qiling/commit/eb2477b0a093f5d8172a489b8f20f5be7df37e10) | Using the advance LCD1602 in example | Authored commit |
| [`ab574671d7`](https://github.com/qilingframework/qiling/commit/ab574671d7c724be5411a4635a5c2e3c365e12a6) | Integrate LCD1602 in device | Authored commit |
| [`ae8932dcde`](https://github.com/qilingframework/qiling/commit/ae8932dcdeabe7065507eec2df5f83cc3716ed9b) | Fix the test for new api | Authored commit |
| [`2b8b39e4eb`](https://github.com/qilingframework/qiling/commit/2b8b39e4eb379bb33035bf35f761265a595c4091) | Add step api for external device | Authored commit |
| [`c92c386878`](https://github.com/qilingframework/qiling/commit/c92c386878e8ee769c830190fe1c7c79deefdda9) | Create the external device module | Authored commit |
| [`5576605be1`](https://github.com/qilingframework/qiling/commit/5576605be146e7f0e4b558a86b9f0a22d4948fce) | Merge branch 'dev' of https://github.com/cla7aye15I4nd/qiling into dev | Authored commit |
| [`f627553fdf`](https://github.com/qilingframework/qiling/commit/f627553fdf371b776c1ca7aae2ef26dad8a84a69) | Refactor the tube design | Authored commit |
| [`21eb482d21`](https://github.com/qilingframework/qiling/commit/21eb482d21a1afd8a9ce3f022b40a2ea0eb9e30a) | Fix the device limit for I2C | Authored commit |
| [`38564fd8bf`](https://github.com/qilingframework/qiling/commit/38564fd8bfa4db6725aa0d4edd69fb7bc48fbff1) | Merge pull request #971 from cla7aye15I4nd/dev | Authored commit |
| [`66d2cc3897`](https://github.com/qilingframework/qiling/commit/66d2cc3897cb9a5e58339edfab1344a81165e04d) | Fix the LCD example | Authored commit |
| [`b02ff6542f`](https://github.com/qilingframework/qiling/commit/b02ff6542fe27f10e764a4973503b6ed9205db7b) | Adjust the call sequence | Authored commit |
| [`203b7e8869`](https://github.com/qilingframework/qiling/commit/203b7e88698a39fac9511a3346195d63acda1aeb) | Add device support for USART, I2C and SPI | Authored commit |
| [`f6c4d2fb76`](https://github.com/qilingframework/qiling/commit/f6c4d2fb7629a883fd86cdfa7504ef4c8d71bd1d) | Add support for device connect | Authored commit |
| [`6f2670eae5`](https://github.com/qilingframework/qiling/commit/6f2670eae55ea96c8980903a87f02814ce8d55a7) | Merge branch 'dev' of https://github.com/cla7aye15I4nd/qiling into dev | Authored commit |
| [`efbb1c063c`](https://github.com/qilingframework/qiling/commit/efbb1c063c68ed49fb489e17ca8d4670d4921362) | Thread safe pipe for connectivity periperhal IO | Authored commit |
| [`07a08e05b5`](https://github.com/qilingframework/qiling/commit/07a08e05b51048b7bf0efdc0db6983b87c861ead) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`a4522ecca1`](https://github.com/qilingframework/qiling/commit/a4522ecca190445a3cdfd3c328f0e06ffcc0d991) | The RTC pass the initlization stage | Authored commit |
| [`dfcdf62752`](https://github.com/qilingframework/qiling/commit/dfcdf627526cd5c0b25af15be02065c7229f7fae) | Add BCD format utils | Authored commit |
| [`c63335bd55`](https://github.com/qilingframework/qiling/commit/c63335bd55242d1e177e7181896e474f86fd1490) | Add missing I2c Interrupt | Authored commit |
| [`f009b387fe`](https://github.com/qilingframework/qiling/commit/f009b387fe51961e0c2d2fd9e475511225d32a5e) | The RTC is harder than I think | Authored commit |
| [`3bdec8eabe`](https://github.com/qilingframework/qiling/commit/3bdec8eabefd94c71e838f01d76c1ec48d74db18) | Add BCD util tools | Authored commit |
| [`ee6eec440d`](https://github.com/qilingframework/qiling/commit/ee6eec440d7c471593bd23e822d7bd562b4eff41) | RTC has cheated the MCU | Authored commit |
| [`492bb1bcb9`](https://github.com/qilingframework/qiling/commit/492bb1bcb95d3125cebca12fe45f7baa867a92f0) | Merge pull request #969 from cla7aye15I4nd/dev | Authored commit |
| [`5349a26411`](https://github.com/qilingframework/qiling/commit/5349a2641181aad3a9d62f19a870776d8e28571a) | Generate the RTC register const | Authored commit |
| [`a2113bccf2`](https://github.com/qilingframework/qiling/commit/a2113bccf2de121d98e9781670520bf3ef872f63) | Merge branch 'dev' of https://github.com/cla7aye15I4nd/qiling into dev | Authored commit |
| [`4f5c3d87a8`](https://github.com/qilingframework/qiling/commit/4f5c3d87a8c6cbb978c7320c3f9d9f87c90c1cac) | Use the new reigster const in DMA | Authored commit |
| [`def1307dbc`](https://github.com/qilingframework/qiling/commit/def1307dbc53f664006ac5adda12ec76a10c1776) | Generate the DMA reigster const | Authored commit |
| [`eba446ea5c`](https://github.com/qilingframework/qiling/commit/eba446ea5c5f16574b71cadd592671cc91cc2c29) | Add USART register mask const | Authored commit |
| [`129d1ebf00`](https://github.com/qilingframework/qiling/commit/129d1ebf00b6354fa2f0e0ebc17b078e37b0e417) | Add the ignored rdyon bit | Authored commit |
| [`13d68ca209`](https://github.com/qilingframework/qiling/commit/13d68ca209c588ce0527a53935eee9d641abef98) | Add RCC register bit const | Authored commit |
| [`936469f802`](https://github.com/qilingframework/qiling/commit/936469f802419ec799f9b277253a1737ee37c71d) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`6d0828a992`](https://github.com/qilingframework/qiling/commit/6d0828a992be9a87b83598f295a4444128ae23da) | tidy up mcu examples | Authored commit |
| [`e8d040c81c`](https://github.com/qilingframework/qiling/commit/e8d040c81c342cefb7a969f513504a36d70dee95) | Add logger switch option | Authored commit |
| [`472bf4e38f`](https://github.com/qilingframework/qiling/commit/472bf4e38f27e475ad7723ccfba4caca755d936f) | Delete the repeat logger | Authored commit |
| [`106cebb430`](https://github.com/qilingframework/qiling/commit/106cebb4300b711e4d38464867bf1d376d3a9dab) | Apply the new decrator | Authored commit |
| [`42d76c71c1`](https://github.com/qilingframework/qiling/commit/42d76c71c1a27d9042004de8a94acaf3e614d2bb) | Combine the two debug decorator | Authored commit |
| [`a7bf222793`](https://github.com/qilingframework/qiling/commit/a7bf222793857fbddca690f240bb9e7286ffb8b7) | Fix the debug output of DMA | Authored commit |
| [`8fb73ef4d4`](https://github.com/qilingframework/qiling/commit/8fb73ef4d48810b470a87afca02768d65e3c18d7) | Merge pull request #968 from cla7aye15I4nd/dev | Authored commit |
| [`0cf8ecd959`](https://github.com/qilingframework/qiling/commit/0cf8ecd959f7dbf4390ff40778832230f51d2c56) | Test the USART crash bug | Authored commit |
| [`c57879c93d`](https://github.com/qilingframework/qiling/commit/c57879c93d144aaa3a97a13bfa26cbc5e3b7e8ec) | Add peripheral read value debug info | Authored commit |
| [`e3c978472b`](https://github.com/qilingframework/qiling/commit/e3c978472b4ad67f1860370aa36ff1bb6c8b1b26) | Apply the peripheral read/write debug decorator | Authored commit |
| [`4acb5e58f1`](https://github.com/qilingframework/qiling/commit/4acb5e58f1420d769cfc34fd08d0d08136966a82) | Add debug decorator | Authored commit |
| [`d479d7a9a0`](https://github.com/qilingframework/qiling/commit/d479d7a9a0ea7eec67e3c2d72dcfa7479bfb992f) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`d939f0a1a4`](https://github.com/qilingframework/qiling/commit/d939f0a1a411dab314291242d934591d95926948) | Fix the merge process | Authored commit |
| [`1d68923bc8`](https://github.com/qilingframework/qiling/commit/1d68923bc8fd5f730062b7d2bff20132cac5c1b7) | Merge branch 'dev' of https://github.com/cla7aye15I4nd/qiling into dev | Authored commit |
| [`f058e67d17`](https://github.com/qilingframework/qiling/commit/f058e67d17278fd6e60aeb140c55a0acf70b35dc) | Handle the interrupt infinite loop | Authored commit |
| [`19646aecb3`](https://github.com/qilingframework/qiling/commit/19646aecb3b80eb309e04c89d36095ec32190331) | Split the arch and interrupt handling | Authored commit |
| [`b1b3e73119`](https://github.com/qilingframework/qiling/commit/b1b3e73119859b104e413ca68091f0cbe53e70e1) | Handle the interrupt block | Authored commit |
| [`978af70ff6`](https://github.com/qilingframework/qiling/commit/978af70ff69516c49c60ecb56b710917b26a1883) | Merge branch 'dev' of https://github.com/cla7aye15I4nd/qiling into dev | Authored commit |
| [`772d274d00`](https://github.com/qilingframework/qiling/commit/772d274d00c04d10d1b8b7c7b730818029308a32) | Fix the usart rw order bug | Authored commit |
| [`20af32e2d2`](https://github.com/qilingframework/qiling/commit/20af32e2d2fc149d8c94639ab2a89c2f5888f7ce) | Merge pull request #960 from cla7aye15I4nd/dev | Authored commit |
| [`97a50381dd`](https://github.com/qilingframework/qiling/commit/97a50381dd7f61a92fd64e68e5c24199c381594a) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`6e54620d87`](https://github.com/qilingframework/qiling/commit/6e54620d87f0e09e089d3a5ff1da612e0c575f2d) | Fix the debug output of UART | Authored commit |
| [`efb88c9307`](https://github.com/qilingframework/qiling/commit/efb88c930792997b6e7b1fa3cfa1f41fa2ebbf91) | Merge pull request #953 from cla7aye15I4nd/dev | Authored commit |
| [`9ddceea833`](https://github.com/qilingframework/qiling/commit/9ddceea8339624e7b1c542902b3b2629e34f9469) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`d4e0b0f782`](https://github.com/qilingframework/qiling/commit/d4e0b0f782ab12cb4b3d94aeb4f4680088c77cdb) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`cfac3238c3`](https://github.com/qilingframework/qiling/commit/cfac3238c37b68596b31c066222e6f77f9dbb178) | Add stm32f407 testcase | Authored commit |
| [`a117346f47`](https://github.com/qilingframework/qiling/commit/a117346f47e9e739e9549cba9ff8ca19296dbcc1) | Add `set_ratio` in systick | Authored commit |
| [`4a1418a4dd`](https://github.com/qilingframework/qiling/commit/4a1418a4dde4ea668228405052284b36db3803f6) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`7a81888997`](https://github.com/qilingframework/qiling/commit/7a818889979f14a2674759756b204926e65fe0bf) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`f7a6352af1`](https://github.com/qilingframework/qiling/commit/f7a6352af1326dd89497bf2bbb5ea91698b08f5e) | Fix typo in const.py | Authored commit |
| [`6184baf83a`](https://github.com/qilingframework/qiling/commit/6184baf83abb6bed82a8dfc0d2edbe01f534b324) | Add docstring in qlhwmanager | Authored commit |
| [`06a50638ff`](https://github.com/qilingframework/qiling/commit/06a50638ffa0350d9641dc14a8bcee05c3203e15) | Add docstring for Qlperipheral | Authored commit |
| [`a050927dcc`](https://github.com/qilingframework/qiling/commit/a050927dccaca6ff865e43d628a4ed92f1f5095d) | Add type annotation for read/write function in hw | Authored commit |
| [`b73ff548f2`](https://github.com/qilingframework/qiling/commit/b73ff548f2c9bbc6c3d053cd4724bc4f5b6987c9) | Use the python3.8 feature to simplify code | Authored commit |
| [`5b86c25669`](https://github.com/qilingframework/qiling/commit/5b86c25669b2a155b76b6cb901aa9a596cdeb7d2) | Remove 'end' field in Qiling | Authored commit |
| [`96c2c6c9dd`](https://github.com/qilingframework/qiling/commit/96c2c6c9ddbfd93eec7279e7a0819d74dfe9bf90) | Import the code convention | Authored commit |
| [`41a548e739`](https://github.com/qilingframework/qiling/commit/41a548e7391041585e25700e395d2d58d23e70f8) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`af7f9a5fdb`](https://github.com/qilingframework/qiling/commit/af7f9a5fdb0a002640367db722e1f7c6e138a012) | Enable the mcu test in script | Authored commit |
| [`8663259aa7`](https://github.com/qilingframework/qiling/commit/8663259aa7534714ca3c65faff5b2b770a26829d) | Add MCU testcase | Authored commit |
| [`7b519ed546`](https://github.com/qilingframework/qiling/commit/7b519ed546e4e518ec9f04f96d53948c2cd22fe9) | Remove the self import | Authored commit |
| [`e8f6976c7a`](https://github.com/qilingframework/qiling/commit/e8f6976c7a989fb71232e3a48686ac90d27657b9) | Add MCU examples | Authored commit |
| [`9caf017120`](https://github.com/qilingframework/qiling/commit/9caf0171205ab417cbf755659349a3e1f881dfcd) | Add stm32f4 series profiles | Authored commit |
| [`113ead06e7`](https://github.com/qilingframework/qiling/commit/113ead06e7f3b546ddb67d95e9a705fde07f9b33) | Enable the MCU feature | Authored commit |
| [`1483c710c4`](https://github.com/qilingframework/qiling/commit/1483c710c411614a1bd8f146b1ea049dc8fd81df) | Add MCU Loader | Authored commit |
| [`ab51ee6d88`](https://github.com/qilingframework/qiling/commit/ab51ee6d88440bc25a98200be0fa4ff2afa18a94) | Add support of Cortex-M | Authored commit |
| [`41459c5b20`](https://github.com/qilingframework/qiling/commit/41459c5b2055c85c1cfb34af77537c7be2c0aa9d) | Introduce MMIO mechanism in memory | Authored commit |
| [`754536515d`](https://github.com/qilingframework/qiling/commit/754536515d1445a80c94b89147ccc0ef3f9e10a7) | Add hw component in qiling | Authored commit |
| [`b40e5670d2`](https://github.com/qilingframework/qiling/commit/b40e5670d28442c75f8aa7b0f635ee3cc24f983e) | Merge branch 'dev' into dev | Authored commit |
| [`e36f0189aa`](https://github.com/qilingframework/qiling/commit/e36f0189aafc33fa23b9018af3b6f685074217b6) | Merge from 'qiling/dev' | Authored commit |
| [`53759504a4`](https://github.com/qilingframework/qiling/commit/53759504a4153da8a3ab50a8cfcbcfdabf553e28) | Fix the typo of test | Authored commit |
| [`5c884c4a6e`](https://github.com/qilingframework/qiling/commit/5c884c4a6ee0d154e5b3202ceb2b9ed6e894c0cd) | Add ping test | Authored commit |
| [`6f37ccbd23`](https://github.com/qilingframework/qiling/commit/6f37ccbd2396584221c20f864bf5742d2fcd26a4) | Merge branch 'qilingframework:dev' into dev | Authored commit |
| [`b647fd3c81`](https://github.com/qilingframework/qiling/commit/b647fd3c81292858ce2b0175b3e6cd42864850f3) | Improved network system call, '/bin/ping' can works now | Authored commit |
| [`538ddc74fb`](https://github.com/qilingframework/qiling/commit/538ddc74fb4d45c82d3a9ed1831a8ffcc740b27f) | Fix the time syscall bug | Authored commit |
| [`62346715d6`](https://github.com/qilingframework/qiling/commit/62346715d6a078064456fb3fd6f13e850f96e048) | Let the output like strace | Authored commit |
| [`e3926fff2f`](https://github.com/qilingframework/qiling/commit/e3926fff2fafb68e71cac918e1acb92ea7637d1a) | Build the cloexec test | Authored commit |
| [`7a60153949`](https://github.com/qilingframework/qiling/commit/7a601539499b932245ca43d234e2bc61a1434376) | Now, the Gzip can work without the bug of (open/unlink)at | Authored commit |
| [`1a08c07061`](https://github.com/qilingframework/qiling/commit/1a08c07061c0b3876b8a5500a057b55606e80e9d) | Some missing linux syscalls | Authored commit |
| [`bfb3a77a3f`](https://github.com/qilingframework/qiling/commit/bfb3a77a3f14a945b656c9055a99899093608b9d) | Be consistent with linux | Authored commit |
| [`cbd22a9409`](https://github.com/qilingframework/qiling/commit/cbd22a9409a5ef5fc4d544d7fa70cdb8ddd3321a) | Replace the magic number with NR_OPEN | Authored commit |
| [`106e3fabc2`](https://github.com/qilingframework/qiling/commit/106e3fabc269d68bc762eec600ed5b7e00f3697a) | Moved the close-on-exec execution position | Authored commit |
| [`dc6d787679`](https://github.com/qilingframework/qiling/commit/dc6d78767984dcaa41ef94677c403923ac48428f) | Avoid some custom situations | Authored commit |
| [`7cd2426dd0`](https://github.com/qilingframework/qiling/commit/7cd2426dd00010f0bcc24271580baff2c8b15908) | Add basic support for the close-on-exec flag | Authored commit |
| [`83da6515ed`](https://github.com/qilingframework/qiling/commit/83da6515ed4d91296c91e3928ca4e83f9e4db944) | Add some relocation types (x86) | Authored commit |
| [`00760d170e`](https://github.com/qilingframework/rootfs/commit/00760d170e46095fcff97f79421262ef0e75d901) | Revert "Delete wrong firmware" | Authored commit |
| [`bec323bf49`](https://github.com/qilingframework/rootfs/commit/bec323bf49a7d129936bcbb2d6df4ea0eaf24cbd) | Add an overflow example | Authored commit |
| [`f66b568d41`](https://github.com/qilingframework/rootfs/commit/f66b568d41f1d1b97d0c4151f5acc9b2aea04a0e) | Delete wrong firmware | Authored commit |
| [`0665589bec`](https://github.com/qilingframework/rootfs/commit/0665589bec772a75fae97e088a338f62aab91d42) | Add basic sd card firmware | Authored commit |
| [`d8d54fcd08`](https://github.com/qilingframework/rootfs/commit/d8d54fcd0835b9bcdbb146e9f277fc2eb69ff79f) | Add Arduino Due example | Authored commit |
| [`2c1aa456c2`](https://github.com/qilingframework/rootfs/commit/2c1aa456c249e8fdeb5383233a7e45e0b791cb56) | Add SCTF stm32f103 example | Authored commit |
| [`3a1e3352cf`](https://github.com/qilingframework/rootfs/commit/3a1e3352cfa20dfecbd452b5bcdd210408bf2765) | Add MNIST examples (STM32F407 + OLED12864) | Authored commit |
| [`24a743372c`](https://github.com/qilingframework/rootfs/commit/24a743372c8115000231e4da0d5a939e84d30129) | STM32 ML examples (crc testcase) | Authored commit |
| [`ceca1d03e0`](https://github.com/qilingframework/rootfs/commit/ceca1d03e03032e533a5f3ae7db7cea972211d75) | Add OLED12864 example | Authored commit |
| [`6bce8cf78e`](https://github.com/qilingframework/rootfs/commit/6bce8cf78e7cb11b7df0244237d9e3070d702305) | Merge branch 'master' of https://github.com/qilingframework/rootfs into HEAD | Authored commit |
| [`e5f8053270`](https://github.com/qilingframework/rootfs/commit/e5f80532700696b518c9f1167a803ee391dda788) | Add basic STM32 TIM example | Authored commit |
| [`f91a8fb9ea`](https://github.com/qilingframework/rootfs/commit/f91a8fb9eaaaf77cc805c0ec1794eb5b97c68c7a) | Merge branch 'master' of https://github.com/qilingframework/rootfs into HEAD | Authored commit |
| [`852fd89ccd`](https://github.com/qilingframework/rootfs/commit/852fd89ccd39e52aab817f5b83c16f58b155784b) | Add I2C Interrupt examples | Authored commit |
| [`83d179819f`](https://github.com/qilingframework/rootfs/commit/83d179819f035d960ef3fe90bf61c7e7d63c4121) | Merge branch 'master' of https://github.com/qilingframework/rootfs into HEAD | Authored commit |
| [`b571c03587`](https://github.com/qilingframework/rootfs/commit/b571c035876c34951753e4b552b6719e9ca8b70c) | add gd32 testfile | Authored commit |
| [`c6dc930b68`](https://github.com/qilingframework/rootfs/commit/c6dc930b680fcc1beb6a5c4cbcc1ef7ff82be969) | Fix the riscv32 library version | Authored commit |
| [`42519b1333`](https://github.com/qilingframework/rootfs/commit/42519b1333ba22af7a22b4b1ccc61a2687968010) | riscv dyn test file | Authored commit |
| [`7a7c69efb0`](https://github.com/qilingframework/rootfs/commit/7a7c69efb060ad746969eaf9ec67741de1b3aec6) | Add riscv dyn test file | Authored commit |
| [`9e2f4037fe`](https://github.com/qilingframework/rootfs/commit/9e2f4037fe1129840a581b206e6c68d56f6d3edd) | Add riscv linux env | Authored commit |
| [`9f5c6cbb9c`](https://github.com/qilingframework/rootfs/commit/9f5c6cbb9ccd6cc86effc1409adbbf164b6596c0) | usart rust testcase (interrupt bug) | Authored commit |
| [`224b431075`](https://github.com/qilingframework/rootfs/commit/224b431075576a3820953defbbbfbb645aef7a1f) | STM32 LED example compiled by Rust | Authored commit |
| [`3ebd7f0565`](https://github.com/qilingframework/rootfs/commit/3ebd7f056596e26293ab8b79015bc8f21b35698a) | LCD Advance Example | Authored commit |
| [`0561171907`](https://github.com/qilingframework/rootfs/commit/0561171907e6c6c0eba7d5d6f50bc8636f02106b) | Merge branch 'qilingframework:master' into master | Authored commit |
| [`edcbee0b40`](https://github.com/qilingframework/rootfs/commit/edcbee0b4084a704e9ac192435ea5d4962280b12) | Add SPI simple test | Authored commit |
| [`ce3e6c6f07`](https://github.com/qilingframework/rootfs/commit/ce3e6c6f076456d54ffc7043837ae6b09799cb05) | Add I2C-LCD testcase | Authored commit |
| [`3bbfcbd46f`](https://github.com/qilingframework/rootfs/commit/3bbfcbd46f043c0033e8cffdf46c9d6ce8646e92) | Merge branch 'qilingframework:master' into master | Authored commit |
| [`92e4863740`](https://github.com/qilingframework/rootfs/commit/92e48637406c2570fa357b250b93e80a2d301b15) | Merge branch 'master' of https://github.com/cla7aye15I4nd/rootfs | Authored commit |
| [`bf8938b3f5`](https://github.com/qilingframework/rootfs/commit/bf8938b3f5afc563c23f45729883fda5cdf5d254) | Add DMA and Timer testcase | Authored commit |
| [`225f511818`](https://github.com/qilingframework/rootfs/commit/225f511818c8f225b6b3de00a7f1bbe983979515) | Merge branch 'qilingframework:master' into master | Authored commit |
| [`a3e0d6235e`](https://github.com/qilingframework/rootfs/commit/a3e0d6235ef28d4f16af7b9925e3cd79f06393ea) | Recompile the FreeRTOS testcase with shorter sleep time | Authored commit |
| [`4b7bad57bf`](https://github.com/qilingframework/rootfs/commit/4b7bad57bf08d966a73231f540cea9971d996c2e) | Add FreeRTOS as MCU test | Authored commit |
| [`010a2a0fa4`](https://github.com/qilingframework/rootfs/commit/010a2a0fa44b505eb91390c9074ed883c188dce1) | Add stm32f407 example | Authored commit |
| [`979a6e18f9`](https://github.com/qilingframework/rootfs/commit/979a6e18f9dd834c74f2df63b8e5a937e24d7fb1) | Merge branch 'qilingframework:master' into master | Authored commit |
| [`a8b578598b`](https://github.com/qilingframework/rootfs/commit/a8b578598b329e0c3714ce3a92a12699411d869a) | Add md5_server test | Authored commit |
| [`032ec7176f`](https://github.com/qilingframework/rootfs/commit/032ec7176f62af851d6cd30579b69ea15efb0453) | Merge branch 'qilingframework:master' into master | Authored commit |
| [`9cf9a16325`](https://github.com/qilingframework/rootfs/commit/9cf9a163254831ad627a862876100d33cbe77bb5) | Merge branch 'master' of https://github.com/cla7aye15I4nd/rootfs | Authored commit |
| [`f7f0b6bd2a`](https://github.com/qilingframework/rootfs/commit/f7f0b6bd2ad004b6c0bfdebb64c2a3d9ae160062) | Add uart testcase | Authored commit |
| [`f7da4589ac`](https://github.com/qilingframework/rootfs/commit/f7da4589ac9b98f7cebb83b55765ca9cb3d23736) | Merge branch 'qilingframework:master' into master | Authored commit |
| [`34759c14ea`](https://github.com/qilingframework/rootfs/commit/34759c14ead315db5916c9d50daafbf494b0517a) | stm32 example | Authored commit |
| [`558c25cf89`](https://github.com/qilingframework/rootfs/commit/558c25cf89fde1105b580fe71456e29fae36b833) | Add ping-test's binary and dependent libraries | Authored commit |
| [`b013ad9bef`](https://github.com/qilingframework/rootfs/commit/b013ad9bef664ecb4b05400eaa8533cc5e0a9f6d) | Add cloexec test binary | Authored commit |

</details>

### Sentry

[Project repository](https://github.com/getsentry/sentry-python)

<details>
<summary>Pull requests (1)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [fix(openai): Guard against `choices=None`](https://github.com/getsentry/sentry-python/pull/6216) | Merged | Upstream: `getsentry/sentry-python` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`640c48d444`](https://github.com/getsentry/sentry-python/commit/640c48d444c2e90d7a42d6f85e9e571cd9e9c88b) | fix(openai): Guard against `choices=None` (#6216) | Authored commit |

</details>

### ShivyC

[Project repository](https://github.com/ShivamSarodia/ShivyC)

<details>
<summary>Pull requests (1)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Delete a useless line of code](https://github.com/ShivamSarodia/ShivyC/pull/111) | Merged | Upstream: `ShivamSarodia/ShivyC` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`e7d72eff23`](https://github.com/ShivamSarodia/ShivyC/commit/e7d72eff237e1ef49ec70333497348baf86be425) | Delete a useless line of code (#111) | Authored commit |

</details>

### sqlite3-ruby

[Project repository](https://github.com/sparklemotion/sqlite3-ruby)

- [GHSA-j7fr-3v8c-3qc3](https://github.com/advisories/GHSA-j7fr-3v8c-3qc3) — sqlite3-ruby has Use-After-Free in SQLite Aggregate Function Callbacks. Official reporter credit; fixed in 2.9.5.
- [GHSA-28hh-pr2h-2w89](https://github.com/advisories/GHSA-28hh-pr2h-2w89) — sqlite3-ruby has Use-After-Free When Redefining SQLite Functions with Different Arity. Official reporter credit; fixed in 2.9.5.

<details>
<summary>Commits and patchsets (2)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`b24e1e6076`](https://github.com/sparklemotion/sqlite3-ruby/commit/b24e1e6076528b7f95f99acf7a81c70d0004c726) | Fix referenced by GHSA-j7fr-3v8c-3qc3 | Reporter credit; maintainer-authored fix |
| [`2bd436d17f`](https://github.com/sparklemotion/sqlite3-ruby/commit/2bd436d17f77cdd4c31b00fe9d50b0d21cbaf033) | Fix referenced by GHSA-28hh-pr2h-2w89 | Reporter credit; maintainer-authored fix |

</details>

### TileLang

[Project repository](https://github.com/tile-ai/tilelang)

<details>
<summary>Pull requests (9)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [\[BugFix\] Handle strided global buffers correctly in 1D TMA copies](https://github.com/tile-ai/tilelang/pull/2746) | Merged | Upstream: `tile-ai/tilelang` | cla7aye15I4nd |
| [\[BugFix\] Preserve re-evaluation of mutable if conditions](https://github.com/tile-ai/tilelang/pull/2744) | Merged | Upstream: `tile-ai/tilelang` | cla7aye15I4nd |
| [\[BugFix\] Preserve loop steps during unswitching](https://github.com/tile-ai/tilelang/pull/2741) | Merged | Upstream: `tile-ai/tilelang` | cla7aye15I4nd |
| [\[BugFix\] Use callee global symbols for cross-target calls](https://github.com/tile-ai/tilelang/pull/2740) | Merged | Upstream: `tile-ai/tilelang` | cla7aye15I4nd |
| [\[BugFix\] Emit Metal barriers for dynamic shared memory](https://github.com/tile-ai/tilelang/pull/2738) | Merged | Upstream: `tile-ai/tilelang` | cla7aye15I4nd |
| [\[BugFix\] Honor explicit row strides in Metal GEMM](https://github.com/tile-ai/tilelang/pull/2730) | Merged | Upstream: `tile-ai/tilelang` | cla7aye15I4nd |
| [\[BugFix\] Isolate cross-compiler options per invocation](https://github.com/tile-ai/tilelang/pull/2728) | Merged | Upstream: `tile-ai/tilelang` | cla7aye15I4nd |
| [\[BugFix\] Preserve buffer element offsets in access pointers](https://github.com/tile-ai/tilelang/pull/2727) | Merged | Upstream: `tile-ai/tilelang` | cla7aye15I4nd |
| [\[BugFix\] Fix HIP predicated dword copy zero fill](https://github.com/tile-ai/tilelang/pull/2721) | Merged | Upstream: `tile-ai/tilelang` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (9)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`5ef1500ed2`](https://github.com/tile-ai/tilelang/commit/5ef1500ed27add9adc3e58fed0e809219edea345) | \[BugFix\] Handle strided global buffers correctly in 1D TMA copies (#2746) | Authored commit |
| [`1591d368db`](https://github.com/tile-ai/tilelang/commit/1591d368dbbd3b2001132e13cad23449210215d3) | \[BugFix\] Preserve re-evaluation of mutable if conditions (#2744) | Authored commit |
| [`235077cb58`](https://github.com/tile-ai/tilelang/commit/235077cb5835c6a3632544f1cb4ec8acc396ac28) | \[BugFix\] Preserve loop steps during unswitching (#2741) | Authored commit |
| [`390d208db3`](https://github.com/tile-ai/tilelang/commit/390d208db378ba0f6f65142460e3a9045c28874a) | \[BugFix\] Use callee global symbols for cross-target calls (#2740) | Authored commit |
| [`0c88682f6f`](https://github.com/tile-ai/tilelang/commit/0c88682f6f216e4a7d02d453cdc2cbc18bf75c5d) | \[BugFix\] Emit Metal barriers for dynamic shared memory (#2738) | Authored commit |
| [`512d51f518`](https://github.com/tile-ai/tilelang/commit/512d51f518113bc40545b7dd808d07ec7e1e4393) | \[BugFix\] Honor explicit row strides in Metal GEMM (#2730) | Authored commit |
| [`322a9cbb6e`](https://github.com/tile-ai/tilelang/commit/322a9cbb6ea771fe4201984f350f343c49f14414) | \[BugFix\] Isolate cross-compiler options per invocation (#2728) | Authored commit |
| [`bd5ca2f05a`](https://github.com/tile-ai/tilelang/commit/bd5ca2f05a384e9ae4cf798e971560c9b0c37608) | \[BugFix\] Preserve buffer element offsets in access pointers (#2727) | Authored commit |
| [`8cfc90e026`](https://github.com/tile-ai/tilelang/commit/8cfc90e026d7a117ed98d1d0cd2f55333b3be6a7) | \[BugFix\] Fix HIP predicated dword copy zero fill (#2721) | Authored commit |

</details>

### Unicorn

[Project repository](https://github.com/unicorn-engine/unicorn)

<details>
<summary>Bug and vulnerability reports (4)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Weird Thing in Cortex-M](https://github.com/unicorn-engine/unicorn/issues/1599) — Fixed; linked by the maintainer or issue closing event. Evidence: [fix commit](https://github.com/unicorn-engine/unicorn/commit/4e227446791e1881e7da4f3ce73c941d233e44cf), [maintainer response](https://github.com/unicorn-engine/unicorn/issues/1599#issuecomment-1109130801).
- [\[ARM\] Missing instructions](https://github.com/unicorn-engine/unicorn/issues/1514) — Fixed; linked by the maintainer or issue closing event. Evidence: [fix commit](https://github.com/unicorn-engine/unicorn/commit/cddc9cf2ede8d6c388e85c3828aec8a3004cfdb0), [maintainer response](https://github.com/unicorn-engine/unicorn/issues/1514#issuecomment-995760064), [maintainer response](https://github.com/unicorn-engine/unicorn/issues/1514#issuecomment-1000945649).
- [Wrong offset in risc-v mmio](https://github.com/unicorn-engine/unicorn/issues/1485) — Fixed; linked by the maintainer or issue closing event. Evidence: [fix commit](https://github.com/unicorn-engine/unicorn/commit/fc467edbc601601ab6ae45d3d7ca49d0fd28b861), [maintainer response](https://github.com/unicorn-engine/unicorn/issues/1485#issuecomment-970706032).
- [\[RISC-V\] `pc` is not increased after execute `ecall`](https://github.com/unicorn-engine/unicorn/issues/1477) — Fixed; linked by the maintainer or issue closing event. Evidence: [fix commit](https://github.com/unicorn-engine/unicorn/commit/67e2386da6eb153e43a2f8bce36552ece33a3821), [maintainer response](https://github.com/unicorn-engine/unicorn/issues/1477#issuecomment-960000899).

</details>

<details>
<summary>Commits and patchsets (4)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`4e22744679`](https://github.com/unicorn-engine/unicorn/commit/4e227446791e1881e7da4f3ce73c941d233e44cf) | Fix linked to issue #1599: Weird Thing in Cortex-M | Reported bug; maintainer-authored fix |
| [`cddc9cf2ed`](https://github.com/unicorn-engine/unicorn/commit/cddc9cf2ede8d6c388e85c3828aec8a3004cfdb0) | Fix linked to issue #1514: \[ARM\] Missing instructions | Reported bug; maintainer-authored fix |
| [`fc467edbc6`](https://github.com/unicorn-engine/unicorn/commit/fc467edbc601601ab6ae45d3d7ca49d0fd28b861) | Fix linked to issue #1485: Wrong offset in risc-v mmio | Reported bug; maintainer-authored fix |
| [`67e2386da6`](https://github.com/unicorn-engine/unicorn/commit/67e2386da6eb153e43a2f8bce36552ece33a3821) | Fix linked to issue #1477: \[RISC-V\] `pc` is not increased after execute `ecall` | Reported bug; maintainer-authored fix |

</details>

### Wasm3

[Project repository](https://github.com/wasm3/wasm3)

<details>
<summary>Pull requests (3)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Fix Heap Buffer Overflow on "DeallocateSlot" Function](https://github.com/wasm3/wasm3/pull/508) | Merged | Upstream: `wasm3/wasm3` | cla7aye15I4nd |
| [Fix Null Pointer Dereference on "main" Function](https://github.com/wasm3/wasm3/pull/507) | Merged | Upstream: `wasm3/wasm3` | cla7aye15I4nd |
| [Fix Global Buffer Overflow on "PreserveRegisterIfOccupied" Function](https://github.com/wasm3/wasm3/pull/506) | Merged | Upstream: `wasm3/wasm3` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (3)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`a027ce3aca`](https://github.com/wasm3/wasm3/commit/a027ce3aca29e4376e4beed784c0571e5a6b39b5) | Fix Null Pointer Dereference on "main" Function (#507) | Authored commit |
| [`d0b5c7e731`](https://github.com/wasm3/wasm3/commit/d0b5c7e7313f385f99c35558a93dcf3437016fba) | Fix overflow (#506) | Authored commit |
| [`f710292fb8`](https://github.com/wasm3/wasm3/commit/f710292fb87fadd08de1d632e6328928db9b3631) | Fix Heap Buffer Overflow on "DeallocateSlot" Function (#508) | Authored commit |

</details>

### Wasmtime

[Project repository](https://github.com/bytecodealliance/wasmtime)

<details>
<summary>Bug and vulnerability reports (2)</summary>

Issue status describes the tracker state; it does not by itself indicate acceptance of a proposed fix.

- [Exception Reference Global Panics Coredump Serialization](https://github.com/bytecodealliance/wasmtime/issues/14102) — Report submitted; no specific accepted fix verified yet.
- [Empty Component Panics Native DWARF Compilation](https://github.com/bytecodealliance/wasmtime/issues/14100) — Fixed by an upstream merged PR. Evidence: [fix PR](https://github.com/bytecodealliance/wasmtime/pull/14130), [fix commit](https://github.com/bytecodealliance/wasmtime/commit/a1f7d4c3cb3fa256dfe7823fa15d9e2b03bb569f).

</details>

<details>
<summary>Commits and patchsets (1)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`a1f7d4c3cb`](https://github.com/bytecodealliance/wasmtime/commit/a1f7d4c3cb3fa256dfe7823fa15d9e2b03bb569f) | Fix panic compiling an empty component with debug info | Reported bug; maintainer-authored fix |

</details>

### Yasm

[Project repository](https://github.com/yasm/yasm)

<details>
<summary>Pull requests (4)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Fix null-pointer-dereference in yasm_expr_get_intnum](https://github.com/yasm/yasm/pull/244) | Merged | Upstream: `yasm/yasm` | cla7aye15I4nd · PatchAgent-assisted |
| [Fix handle_dot_label heap-out-of-bound](https://github.com/yasm/yasm/pull/243) | Merged | Upstream: `yasm/yasm` | cla7aye15I4nd · PatchAgent-assisted |
| [Fix use-after-free in yasm_intnum_destroy](https://github.com/yasm/yasm/pull/242) | Merged | Upstream: `yasm/yasm` | cla7aye15I4nd · PatchAgent-assisted |
| [Fix nullptr deref in yasm_expr__copy_except](https://github.com/yasm/yasm/pull/241) | Merged | Upstream: `yasm/yasm` | cla7aye15I4nd · PatchAgent-assisted |

</details>

<details>
<summary>Commits and patchsets (4)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`9defefae9f`](https://github.com/yasm/yasm/commit/9defefae9fbcb6958cddbfa778c1ea8605da8b8b) | Fix null-pointer-dereference in yasm_expr_get_intnum (#244) | Authored commit |
| [`ecb47f1c87`](https://github.com/yasm/yasm/commit/ecb47f1c8786b4628d5cd718cdccf134ad96e0cb) | Fix handle_dot_label heap-out-of-bound (#243) | Authored commit |
| [`84be2ee6c3`](https://github.com/yasm/yasm/commit/84be2ee6c310607fddbe8154696c9386364679ea) | Fix use-after-free in yasm_intnum_destroy (#242) | Authored commit |
| [`0dfac4d4da`](https://github.com/yasm/yasm/commit/0dfac4d4da1bea4b4f8528cf78df954ef0272a43) | Fix nullptr deref in yasm_expr__copy_except (#241) | Authored commit |

</details>

### PintOS

[Project repository](https://github.com/oscardhc/PintOS)

<details>
<summary>Pull requests (2)</summary>

| PR | Status | Destination | Account / assistance |
| --- | --- | --- | --- |
| [Check intr_context when preempt](https://github.com/oscardhc/PintOS/pull/2) | Merged | Upstream: `oscardhc/PintOS` | cla7aye15I4nd |
| [Merge threads module](https://github.com/oscardhc/PintOS/pull/1) | Merged | Upstream: `oscardhc/PintOS` | cla7aye15I4nd |

</details>

<details>
<summary>Commits and patchsets (26)</summary>

| Commit | Change | Contribution |
| --- | --- | --- |
| [`2a8a5806e4`](https://github.com/oscardhc/PintOS/commit/2a8a5806e4f5ea0322e9b53db4a70adb40be9e1b) | We Are The Champions!!!!!!!!!!!!!!!!!!!!!!!!! | Authored commit |
| [`5962187eab`](https://github.com/oscardhc/PintOS/commit/5962187eab3c5631f1f1f761324f0855d2242298) | Just 2 fail? | Authored commit |
| [`95fc362839`](https://github.com/oscardhc/PintOS/commit/95fc36283934242bcf67f6b6650a1d5d25dbdefa) | Fail at dir-vine | Authored commit |
| [`5d39c8ae88`](https://github.com/oscardhc/PintOS/commit/5d39c8ae88cf75a1a9e8a2201a36ab417c22eedd) | Merge branch 'filesys-subdirectory' into filesys-module-2ndtry | Authored commit |
| [`4ab419d759`](https://github.com/oscardhc/PintOS/commit/4ab419d759453b9994bb59e30658cf116b462adc) | Update Make.vars | Authored commit |
| [`dba971a318`](https://github.com/oscardhc/PintOS/commit/dba971a318745b19d7e31cbd6a557ded03fb42a2) | Almost Pass Subdir | Authored commit |
| [`48eaf72ba0`](https://github.com/oscardhc/PintOS/commit/48eaf72ba0b167f44c3151ad5ddaa7263abb0e85) | Fix strok_r and add more syscall | Authored commit |
| [`382e58e21f`](https://github.com/oscardhc/PintOS/commit/382e58e21faa9297505857d0193a49266cce46d0) | finish chdir | Authored commit |
| [`f8bb51c5f9`](https://github.com/oscardhc/PintOS/commit/f8bb51c5f9db734485ec06fc36982ff385bc79f1) | mkdir single level (40 fail) | Authored commit |
| [`801874a8c7`](https://github.com/oscardhc/PintOS/commit/801874a8c776746e5b9b116ba18429fc90622af3) | Finish cache (looks like right) | Authored commit |
| [`904a15db06`](https://github.com/oscardhc/PintOS/commit/904a15db06b1e7c9f73fe1db2f7b0fc81361bd52) | Add USERPROG marco | Authored commit |
| [`2644bcee32`](https://github.com/oscardhc/PintOS/commit/2644bcee329f2849dbb43357cf5a6bf3c93faacb) | Check all thread code | Authored commit |
| [`1ed8f74088`](https://github.com/oscardhc/PintOS/commit/1ed8f74088d9abf1b56eb6c2579422eece889340) | The thread list is not a priority queue | Authored commit |
| [`bac9e11bdb`](https://github.com/oscardhc/PintOS/commit/bac9e11bdb9e9309b417a8217bcf60d7658a4e9c) | Merge pull request #2 from oscardhc/threads-module | Authored commit |
| [`6d2192db41`](https://github.com/oscardhc/PintOS/commit/6d2192db41b8289f746077b51d224a3d5be293bc) | Check intr_context when preempt | Authored commit |
| [`e1e6eefa49`](https://github.com/oscardhc/PintOS/commit/e1e6eefa498ac95c19e37d57ad7cf2aa0f98e5dd) | Merge pull request #1 from oscardhc/threads-module | Authored commit |
| [`7047cecb98`](https://github.com/oscardhc/PintOS/commit/7047cecb98d7ef3acdaad2e5e2bf8ae818e7836a) | Pass advance schedule (27/27) | Authored commit |
| [`3556886500`](https://github.com/oscardhc/PintOS/commit/3556886500a76a4e056a21c8d541e03a8b5016fc) | Add fix-point operator | Authored commit |
| [`a4478a34cd`](https://github.com/oscardhc/PintOS/commit/a4478a34cda4007955b1b19b617bc7857ca1b22f) | Optimizer algorithm & Check thread mlfqs | Authored commit |
| [`d488d1e811`](https://github.com/oscardhc/PintOS/commit/d488d1e811c0f6e1c10ee3e824b4ee814c8da2c1) | Pass priority-donate-* (20/27) | Authored commit |
| [`353729f9a6`](https://github.com/oscardhc/PintOS/commit/353729f9a6ab936fb89bc5ff2d90c0ab4d6a8e37) | Thread donate priority | Authored commit |
| [`97a39d5793`](https://github.com/oscardhc/PintOS/commit/97a39d5793305974b94a777c68e4f9e43093de81) | Add thread_preempt function (11/27) | Authored commit |
| [`3dcf07014d`](https://github.com/oscardhc/PintOS/commit/3dcf07014d2b9d85bf9946e0e00e78744f164c9b) | Basic thread priority schedule | Authored commit |
| [`fb86276554`](https://github.com/oscardhc/PintOS/commit/fb8627655414fe5e9802f8da9170038296471505) | Clear redundant init code (init_thread -> memset) | Authored commit |
| [`a3ee2becc9`](https://github.com/oscardhc/PintOS/commit/a3ee2becc928fa95ea2a2b51ea1708ed9dd4f3c1) | Optimize timer_sleep function | Authored commit |
| [`3e0d0784fb`](https://github.com/oscardhc/PintOS/commit/3e0d0784fb38cdab58d5784f0126afbd65db9b16) | Fix compile options | Authored commit |

</details>
