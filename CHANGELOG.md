#### wut 1.7.0

###### New features / improvements
* nn/dlp: Add initial headers by @DaniElectra in https://github.com/devkitPro/wut/pull/389
* nn/dlp: Fix Initialize functions on ServerPrivate by @DaniElectra in https://github.com/devkitPro/wut/pull/390
* nn_ccr: Add `CCRSysSetCurrentLCDMode` and `CCRSysGetCurrentLCDMode` by @Maschell in https://github.com/devkitPro/wut/pull/393
* nsysccr/cdc: Add CCRCDCSysGetInfo by @GaryOderNichts in https://github.com/devkitPro/wut/pull/398* nn_acp: Add ACPRemoveSaveDir* by @Andrew1Hawes in https://github.com/devkitPro/wut/pull/394
* nn_acp: Add various save related functions by @Maschell in https://github.com/devkitPro/wut/pull/396
* Add HDMI CEC functions by @GaryOderNichts in https://github.com/devkitPro/wut/pull/397
* Added `OSSetPerformanceMonitor()`. by @dkosmari in https://github.com/devkitPro/wut/pull/400

###### Fixes and corrections
* coreinit/screen: Swap row and column parameters in OSScreenPutFontEx by @capitalistspz in https://github.com/devkitPro/wut/pull/391
* camera: corrections and comments by @capitalistspz in https://github.com/devkitPro/wut/pull/392
* nn_idb: Fix copy headers, fix nn::idb::IDBReader::Initialize by @Maschell in https://github.com/devkitPro/wut/pull/395
* camera: event argument correction by @capitalistspz in https://github.com/devkitPro/wut/pull/399

## New Contributors
* @dkosmari made their first contribution in https://github.com/devkitPro/wut/pull/400

#### wut 1.6.0

###### New features / improvements
* nn_idb: Implement icon database reading by @Maschell in https://github.com/devkitPro/wut/pull/357
* nn_idb: move include into libraries directory by @Maschell in https://github.com/devkitPro/wut/pull/365
* wut_types: Implement more operators for `WUT_ENUM_BITMASK_TYPE` by @GaryOderNichts in https://github.com/devkitPro/wut/pull/369
* whb/gfx: Use 4:3 TV buffers on 4:3 TVs by @jranderia3 in https://github.com/devkitPro/wut/pull/383

###### Breaking changes
* padscore: rename `nunchuck` -> `nunchuk` in https://github.com/devkitPro/wut/pull/348

###### CafeOS related changes
* More nn_ccr and nsysccr struct/enum fixes by @Maschell in https://github.com/devkitPro/wut/pull/361
* Add functions to control the Eco mode by @Maschell in https://github.com/devkitPro/wut/pull/363
* nn_sl: Fix wrong parameters for nn::sl::LaunchInfoDatabase::Unregister by @Maschell in https://github.com/devkitPro/wut/pull/362
* sysapp: Add all possible "jumpTo" targets for SysAppSettingsArgs by @Maschell in https://github.com/devkitPro/wut/pull/366
* nn_ccr: Add CCRSysSetInitBootFlag and CCRSysInitializeSettings, add CCRCDCUicConfigIdEnum values by @Maschell in https://github.com/devkitPro/wut/pull/364
* padscore: Add more functions and types in https://github.com/devkitPro/wut/pull/348
* nsysccr/cdc: Add language and ext update functions by @GaryOderNichts in https://github.com/devkitPro/wut/pull/368
* coreinit: Add __OSPhysicalToEffectiveCached and __OSPhysicalToEffectiveUncached by @Maschell in https://github.com/devkitPro/wut/pull/367
* coreinit: Add "SavedFrame" related functions by @Maschell in https://github.com/devkitPro/wut/pull/374
* nn_acp: Add ACPGetTitleMetaDir and ACPGetTitleMetaDirByTitleListType by @Maschell in https://github.com/devkitPro/wut/pull/375
* coreinit: Add __FSAShimDecodeIosErrorToFsaStatus by @Maschell in https://github.com/devkitPro/wut/pull/378
* coreinit: add stopwatch.h and stopwatchatomic.h by @capitalistspz in https://github.com/devkitPro/wut/pull/370
* nn_ccr: Add CCRSysCaffeineBootCheckAbort; nsysccr: fix quick start menu value in CCRCDCDrcStateEnum by @Maschell in https://github.com/devkitPro/wut/pull/372
* gx2: add GX2GetMainCoreId by @Maschell in https://github.com/devkitPro/wut/pull/380
* vpad: Add VPADGetButtonProcMode by @Maschell in https://github.com/devkitPro/wut/pull/376
* sndcore2: Update AXTransitionAudioBuffer struct by @Maschell in https://github.com/devkitPro/wut/pull/373
* coreinit: Fix wrong/duplicate OSGetCodegenVirtAddrRange declaration, formatting by @Maschell in https://github.com/devkitPro/wut/pull/371
* avm: Add some missing DRC functions by @Maschell in https://github.com/devkitPro/wut/pull/379
* nsysccr: Add CCRCDCRegister*AttachCallback functions by @Maschell in https://github.com/devkitPro/wut/pull/377
* gx2: Add GX2AllocateTilingApertureEx and GX2FreeTilingAperture by @GaryOderNichts in https://github.com/devkitPro/wut/pull/381
* nsysnet/netconfig: Add SOGetProxyConfig by @GaryOderNichts in https://github.com/devkitPro/wut/pull/382
* gx2: Add GX2GetSystemTVAspectRatio by @GaryOderNichts in https://github.com/devkitPro/wut/pull/384
* nsysccr/cdc: Update CCRCDCDrcStateEnum with test menu names by @GaryOderNichts in https://github.com/devkitPro/wut/pull/386
* More DRX definitions by @team-orangeBlue in https://github.com/devkitPro/wut/pull/385
* nn/uds: Add initial headers by @DaniElectra in https://github.com/devkitPro/wut/pull/387

#### wut 1.5.0

###### New features / improvements
* wutnewlib: implement abort, assert and assert_func by @Maschell in https://github.com/devkitPro/wut/pull/337 and updated for devkitPPC r45.1 in https://github.com/devkitPro/wut/pull/359

###### Bug fixes
* wutmalloc: make sure to set errno properly on error by @Maschell in https://github.com/devkitPro/wut/pull/347

###### CafeOS related changes
* Add missing language/region values to nn::erreula and nn::swkbd by @Maschell in https://github.com/devkitPro/wut/pull/336
* nn_nets2: Add somemopt by @GaryOderNichts in https://github.com/devkitPro/wut/pull/338
* coreinit/im: Add IM_SetDeviceState and missing `IMEvent`s by @GaryOderNichts in https://github.com/devkitPro/wut/pull/343
* Add AVM and TVE headers, functions and enums by @Andrew1Hawes in https://github.com/devkitPro/wut/pull/345
* nn/hpad: Add initial headers by @GaryOderNichts in https://github.com/devkitPro/wut/pull/344
* vpad: Fix documentation for VPADRead return value by @GaryOderNichts in https://github.com/devkitPro/wut/pull/346
* nn/temp: Fix TEMPTargetPreference by @GaryOderNichts in https://github.com/devkitPro/wut/pull/349
* coreinit/mcp: Fix MCPAppType for DRC and DRH by @GaryOderNichts in https://github.com/devkitPro/wut/pull/350
* nsysccr/cdc: Add CCRCDCPerSetUicConfig by @GaryOderNichts in https://github.com/devkitPro/wut/pull/351
* nsysccr/cdc: Add software functions by @GaryOderNichts in https://github.com/devkitPro/wut/pull/353
* nn_ccr/sys: Add fw update functions by @GaryOderNichts in https://github.com/devkitPro/wut/pull/355
* padscore: Add missing functions for 7-controller mode by @GaryOderNichts in https://github.com/devkitPro/wut/pull/352
* nsysccr/cdc: Implement CCRCDCSysSetDrhState by @Maschell in https://github.com/devkitPro/wut/pull/356
* nn/sl: Implement more functions/classes by @Maschell in https://github.com/devkitPro/wut/pull/354
* coreinit: Add MEMCheckExpHeap and MEMCheckHeap by @Maschell in https://github.com/devkitPro/wut/pull/358


#### wut 1.4.0

## What's Changed
* nfc: Add initial header by @GaryOderNichts in https://github.com/devkitPro/wut/pull/321
* nsysccr/cdc: Add CCRCDCWowlWakeDrc and CCRCDCWakeStateEnum by @Andrew1Hawes in https://github.com/devkitPro/wut/pull/320
* Add NTAG by @GaryOderNichts in https://github.com/devkitPro/wut/pull/326
* Add system time update functions by @GaryOderNichts in https://github.com/devkitPro/wut/pull/328
* Update camera.h by @Fangal-Airbag in https://github.com/devkitPro/wut/pull/329
* Add missing GX2 enum values by @GaryOderNichts in https://github.com/devkitPro/wut/pull/327
* Add missing optnames and multicast support by @GaryOderNichts in https://github.com/devkitPro/wut/pull/331
* procui: Fix ProcUIInForeground and ProcUIIsRunning comments by @Andrew1Hawes in https://github.com/devkitPro/wut/pull/330
* Finalize compile commands by @thearst3rd in https://github.com/devkitPro/wut/pull/332

#### wut 1.3.2

* Implement wut_set_thread_specific/wut_get_thread_specific as weak functions by @Maschell in https://github.com/devkitPro/wut/pull/324
* wutdevoptab: Add support for opening files with more flag combinations by @Maschell in https://github.com/devkitPro/wut/pull/322

#### wut 1.3.1

* wutmalloc: Always align allocated memory to 0x40 to match newlib behaviour by @Maschell in https://github.com/devkitPro/wut/pull/316
* devoptab_fsa: use c++ headers by @WinterMute in https://github.com/devkitPro/wut/pull/317
* Implement __syscall_getreent by @GaryOderNichts in https://github.com/devkitPro/wut/pull/318
* coreinit: Add some missing field to the OSThread struct by @Maschell in https://github.com/devkitPro/wut/pull/319

#### wut 1.3.0

###### Important changes

- newlib syscalls refactored for latest devkitPPC

###### CafeOS related changes

coreinit:

- Fix OSDynLoad_Error to be a 32bit value by @Maschell in https://github.com/devkitPro/wut/pull/305
- Fix OSDynLoad_EntryReason values by @exzap in https://github.com/devkitPro/wut/pull/307
- Add MCP_CompatLoadAVFile by @GaryOderNichts in https://github.com/devkitPro/wut/pull/309
- Add KernelInfo0/KernelInfo6 structs by @Maschell in https://github.com/devkitPro/wut/pull/310
- MCP_GetSystemVersion by @GaryOderNichts in https://github.com/devkitPro/wut/pull/311
- Separate vpadbase from vpad by @GaryOderNichts in https://github.com/devkitPro/wut/pull/312
- Add missing MCP functions/enums & add more fields to LaunchInfo struct by @Maschell in https://github.com/devkitPro/wut/pull/313



#### wut 1.2.0

###### Important changes

- wutstdc++: Decrease the stack size for gthread threads from 4 MiB to 128 KiB by @Maschell in https://github.com/devkitPro/wut/pull/269
- coreinit: Change the function declaration of OSDynLoad_FindExport by @gblues in https://github.com/devkitPro/wut/pull/289

###### Important bug fixes

- wutdevoptab: Fix memory leak in open() by @Maschell in https://github.com/devkitPro/wut/pull/261
- wutstdc++: Check if memory allocations were successful on thread creation by @Maschell in https://github.com/devkitPro/wut/pull/268
- wutstdc++: Fix potential memory leak when thread creation fails by @Maschell in https://github.com/devkitPro/wut/pull/271
- wutstdc++: Fix __wut_cond_timedwait by @GaryOderNichts in https://github.com/devkitPro/wut/pull/281
- libwhb: Fix length check in ConsoleAddLine by @Maschell in https://github.com/devkitPro/wut/pull/284
- wutcrt: Fix the trap instruction by @Maschell in https://github.com/devkitPro/wut/pull/302
- whb/console: Add missing MEMRecordStateForFrmHeap by @GaryOderNichts in https://github.com/devkitPro/wut/pull/272

###### New features / improvements

- wutdevoptab: Check size of a read/write before checking the buffer alignment to reduce the number of read/write calls by @Maschell in https://github.com/devkitPro/wut/pull/273
- Add IR support by @GaryOderNichts in https://github.com/devkitPro/wut/pull/288
- Adjust C/C++ flags (disable exceptions/rtti) by @fincs

###### CafeOS related changes

coreinit:

- Add const to paths in coreinit/filesystem.h by @Xpl0itU in https://github.com/devkitPro/wut/pull/262
- Add missing IM_* functions from coreinit by @GaryOderNichts in https://github.com/devkitPro/wut/pull/263
- Add missing FSARequest/FSAResponse structs by @Maschell in https://github.com/devkitPro/wut/pull/270
- Add missing coreinit/context.h include in coreinit/interrupts.h by @Maschell in https://github.com/devkitPro/wut/pull/279
- Update FSStateChangeParams and add offset checks by @NessieHax in https://github.com/devkitPro/wut/pull/287
- Add CopyData functions by @GaryOderNichts in https://github.com/devkitPro/wut/pull/283
- Add OSLaunchTitle* functions by @GaryOderNichts in https://github.com/devkitPro/wut/pull/293
- Add missing (internal) OSDynload structs by @Maschell in https://github.com/devkitPro/wut/pull/296
- Fix missing import in rendevouz.h by @Maschell in https://github.com/devkitPro/wut/pull/297
- Add missing functions for setting the context by @Maschell in https://github.com/devkitPro/wut/pull/298
- Add OSGetCodegenVirtAddrRange by @Maschell in https://github.com/devkitPro/wut/pull/300
- Add __OSConsoleWrite by @Maschell in https://github.com/devkitPro/wut/pull/299
- Add some kernel related functions by @Maschell in https://github.com/devkitPro/wut/pull/295
- Add missing fields and enum definitions to OSThread and OSContext by @Maschell in https://github.com/devkitPro/wut/pull/294
- Add FSARequestChangeOwner by @Xpl0itU in https://github.com/devkitPro/wut/pull/291
- Add more languages to LanguageType by @Xpl0itU in https://github.com/devkitPro/wut/pull/290
- Add smd functions/structs by @GaryOderNichts in https://github.com/devkitPro/wut/pull/301

Other:

- nn_ccr: Add several functions by @GaryOderNichts in https://github.com/devkitPro/wut/pull/264
- nsysccr: Add several functions by @GaryOderNichts in https://github.com/devkitPro/wut/pull/265
- gx2: Add several definitions for Multi/Double DRC mode by @GaryOderNichts in https://github.com/devkitPro/wut/pull/266
- nn::Result: Add missing modules by @GaryOderNichts in https://github.com/devkitPro/wut/pull/267
- nn_nfp: Update functions, structs and add documentation by @GaryOderNichts in https://github.com/devkitPro/wut/pull/275
- nn_nfp: Add declarations for amiibo settings by @GaryOderNichts in https://github.com/devkitPro/wut/pull/277
- sysapp: Add argument functions and _SYSDirectlySwitchTo by @GaryOderNichts in https://github.com/devkitPro/wut/pull/276
- sysapp: Add missing functions and cleanup structs by @GaryOderNichts in https://github.com/devkitPro/wut/pull/282
- camera: Add Camera lib (camera.rpl) by @Fangal-Airbag in https://github.com/devkitPro/wut/pull/280

#### wut 1.1.1
###### Important changes
- Changed license to zlib to avoiding licensing issues when linking against wut in non-GPL projects. (#257)

###### Important bug fixes
- Fixed stack alignment to match PPC EABI requirements and avoid undefined behaviour (#248)
- Fixed lseek implementation which caused undefined behaviour on SEEK_CUR (#253)
- Added fix to prevent file-offset overflow in seek implementation (#254)
- Fixed lseek implementation to work correctly on files opend with O_APPEND (#256)
- Fixed and improved usage of atomics (#258)

###### New features
- Added a trapword to the crt in case a debugger is initalized to allow debugging .rpx compiled with wut (#249)
- Added support for the O_EXCL fopen flag and the following flag combinations: `O_WRONLY | O_CREAT`, `O_WRONLY | O_APPEND` and `O_WRONLY | O_TRUNC` (#250)

###### CafeOS related changes
- Fixed invalid ACPInitialize function declaration (#247)
- Fixed order of arguments for FSOpenFileExAsync (#260)

Thanks to @exjam, @fincs, @GaryOderNichts and @Maschell for their contributions to this release.

#### wut 1.1.0
###### Important bug fixes
- Added wut_load_bounds section to prevent loader bug (thanks @GaryOderNichts)
- Make sure to always read into/write from a properly aligned buffer in the devoptab to avoid heap corruption (thanks @WinterMute, @Maschell)
- Impovements of the devoptab to properly support time and mode information and many more fixes (thanks @Maschell, @Crementif)

###### Major new features
- Moved CMake machinery to devkitPro CMake (thanks @fincs)
- Replaced the CafeOS default heap with a custom one (thanks @GaryOderNichts)

###### Minor new features
- Added support for the Logging Module (thanks @Maschell)
- Added support for nn::erreula library (thanks @exjam)

###### Minor bug fixes
- Fixed potential memory leaks in nn::swkdb. (thanks @exjam)
- Fixed return types and arguments for several sysapp functions (thanks @Maschell)
- Fixed memalign to ensure the size is aligned (thanks @Maschell)
- Added missing FSUnmount on fini (thanks @Maschell)
- Only call FSUnmount if FSMount was successful in devoptab (thanks @Maschell)
- Replaced dynamic allocation of OSMutex with static table to avoid memory leaks (thanks @fincs)
- Fixed syscall_clock implementation (thanks @Maschell)
- Fixed FSError enum (thanks @Maschell)
- Fixed setting the correct directory/file flag in devoptab (thanks @Maschell)
- Enforce ACPGetTitleMetaXml parameter alignment requirement. (thanks @Maschell)
- Fixed OSThreadLink struct (thanks @Maschell)

###### Breaking changes
- The CMPTLaunchTitle function declaration has changed to use uint64_t for the title id (thanks @Xpl0itU)
- Removed nlibcurl
- Added missing parameters to multiple functions (e.g. SYSSwitchTo*/ _SYSLaunch*, FSChangeMode/FSChangeModeAsync, HIDSetIdle) (thanks @Maschell)
- Renamed SYSTEM_APP_ID_HOME_MENU to SYSTEM_APP_ID_WII_U_MENU (thanks @Maschell)

###### CafeOS related changes
- Added FSA structs and function declarations (thanks @Maschell)
- Added mic function declarations (thanks @NessieHax)
- Added missing parameter to FSChangeMode/FSChangeModeAsync (thanks @Maschell)
- Added more coreinit function declarations (thanks @Maschell, @LRFLEW, @NessieHax, @Crementif)
- Added more gx2 function declarations (thanks @GaryOderNichts)
- Added more nn::acp function declarations (thanks @Maschell)
- Added more nn::act function declarations (thanks @Maschell)
- Added more nn::ccr function declarations (thanks @Maschell)
- Added more nn::swkdb function declarations (thanks @Fangal-Airbag, @NessieHax)
- Added more nsyshid function declarations (thanks @Maschell)
- Added more nsyshid function declarations (thanks @Maschell)
- Added more nsysnet function declarations (thanks @Maschell)
- Added more nsysuhs function declarations (thanks @GaryOderNichts)
- Added more padscore function declarations (thanks @LRFLEW)
- Added more procui function declarations (thanks @GaryOderNichts)
- Added more sysapp function declarations (thanks @Maschell)
- Added more vpad function declarations (thanks @Maschell)
- Added nn::cmpt function declarations (thanks @GaryOderNichts)
- Added nn::erreula function declarations (thanks @exjam)
- Added nn::fp function declarations (thanks @NessieHax)
- Added nn::nfp function declarations (thanks @GaryOderNichts)
- Added nn::save function declarations (thanks @GaryOderNichts)
- Added nn::sl function declarations (thanks @Maschell)
- Added nn::spm function declarations (thanks @GaryOderNichts)
- Added nn::temp function declarations (thanks @exjam)
- Added nsyskbd function declarations (thanks @Maschell)

#### wut 1.0.0-beta12
###### Important bug fixes
- Numerous improvements to linking rpl/rpx which fixes C++ exceptions and static constructors not working correctly (thanks @fincs)
- Fix `gettod` implementation returning incorrect time (thanks @GaryOderNichts)
- Fix `nn::Result` to work correctly on big endian (thanks @luigoalma)

###### Major new features
- Add Makefile build system support for producing .wuhb files, a new homebrew app bundle format intended to streamline distribution of ancilliary assets (icons, content files) and compatibility with future homebrew loading solutions (thanks @fincs, @Maschell)
- New POSIX compatible socket implementation which aims to make porting existing code to Wii U seamless (thanks @rw-r-r-0644, @GaryOderNichts, @fincs)

###### Minor bug fixes
- Add missing cleanup of filesystem clients in WHB (thanks @Maschell)
- Optimise `fread`, `fwrite` when the provided buffer is already aligned (thanks @Maschell)

###### CafeOS related changes
- Fix names for `IM{Get,Set}DimEnable{DRC,TV}` (was previously incorrectly capitalised Drc and Tv)
- Add missing enum values in gx2 and improve usage of enums from C++ by adding operator| (thanks @fincs)
- Add missing `FSErrorFlag` type for all filesystem functions (thanks @Maschell)
- Add more coreinit function declarations (thanks @Maschell)
- Add more nn_ac function declarations (thanks @Maschell)
- Add some nsysuhs function declarations (thanks @Maschell)
- Add more sndcore2 function declarations (thanks @GaryOderNichts)
- Add more vpad function declarations (thanks @Crayon2000)

#### wut 1.0.0-beta10
###### Breaking changes
- libwhb's network command server (`WHBCommandServer`) functions and the associated `<whb/commandserver.h>` header have been removed.

###### Deprecations
- The CMake macro `wut_create_rpl` has been re-implemented. The new version doesn't create a build target for the rpx/rpl binary, and only regenerates the rpx/rpl when actually necessary. The new syntax is `wut_create_rpl(<TARGET>)`. Deprecated calls in the form `wut_create_rpl(file.rpx <TARGET>)` will fall through to the old implementation.

###### API additions
- Cafe functions `inet_ntoa_r`, `inet_ntop`, and `inet_pton` have been added to `<nsysnet/socket.h>` (thanks [@Crayon2000](https://github.com/devkitPro/wut/commit/df93bf758f54c1d3a65bc7205a81a6da382c31a0)!)
- Cafe functions `VPADGetTPCalibratedPointEx`, `VPADGetTPCalibrationParam`, and `VPADSetTPCalibrationParam` have been added to `<vpad/input.h>`.
- Cafe functions `OSGetOSID` and `__OSGetProcessSDKVersion` have been added to `<coreinit/systeminfo.h>` (thanks [@Maschell](https://github.com/devkitPro/wut/commit/fe230e06ccf43f3b13d25643399dd9a04bf7eb43)!)
- Cafe function `_SYSGetSystemApplicationTitleId` has been added to `<sysapp/title.h>` (thanks [@Maschell](https://github.com/devkitPro/wut/commit/35c20d8700cddd46f5e37789617629e010a8ad1f)!)
- Cafe functions `SYSGetCallerPFID`, `_SYSGetSystemApplicationTitleIdByProdArea`, and `SYSGetCallerTitleId` have been added `<sysapp/title.h>`.
- Cafe functions `OSReportVerbose`, `OSReportInfo`, and `OSReportWarn` have been added to `<coreinit/debug.h>`.
- New libwhb functions `WHBGfxGetTVColourBuffer`, `WHBGfxGetTVDepthBuffer`, `WHBGfxGetTVContextState`, and equivalents for the DRC, have been added to `<whb/gfx.h>`.
- [Helper functions](https://github.com/devkitPro/wut/commit/f0ed4fb91ff7f738f5e36e54094935530cbbbefe) have been added to `<gx2/shaders.h>` which can look up shader uniforms by name.
- A new header file, `<nn/acp.h>`, has been added for nn_acp's meta.xml functionality (thanks [@Maschell](https://github.com/devkitPro/wut/commit/7f2c9b5d696b609d1be8f95597e4be02097f2608)!)
- Cafe structure `KPADStatus` (from `<padscore/kpad.h>`) has been documented, had accelerometer data added, and had nunchuk-specific values added (thanks [@Crayon2000](https://github.com/devkitPro/wut/commit/78ee1c51bc11ae53edd6b6025f8bdb984e05b497)!)
- Various Cafe structures in `<coreinit/mcp.h>` have been updated with newly-discovered members (thanks [@Maschell](https://github.com/devkitPro/wut/commit/b712686c388a7a9cb0a03a82358386df105ac7f7), [again](https://github.com/devkitPro/wut/commit/d1d2da63adabc55de70e82310f312b1b5fe450c2)!)
- Cafe enum `GX2PrimitiveMode` has been updated to include the `LINES_ADJACENCY`, `LINE_STRIP_ADJACENCY`, `TRIANGLES_ADJACENCY`, `TRIANGLE_STRIP_ADJACENCY`, `RECTS`, and `LINE_LOOP` primitives.

###### Other changes
- Cafe functions throughout the GX2 headers have had `const` applied as appropriate, allowing for better compiler optimisations.
- libwhb's Console and graphics helpers have been refactored to better support Cafe's multitasking and home menu overlay. Applications using WHBConsole can now be backgrounded and resumed without issue.
- Cafe's KPAD library has been documented, WPAD has been partially documented, and various fixes were made to the VPAD documentation (thanks [@Crayon2000](https://github.com/devkitPro/wut/commit/78ee1c51bc11ae53edd6b6025f8bdb984e05b497)!)
- CMake now searches for libraries in internal devkitPPC folders, allowing `find_library(m)` (and CMake pkg-config equivalents) to work as expected.
- CMake now sets the pkg-config binary to `powerpc-eabi-pkg-config`, installable from the `dkp-libs` repo as `wiiu-pkg-config`. Application scripts no longer need to set `PKG_CONFIG_EXECUTABLE`.
- wutstdc++'s threading implementation has been changed to behave more like a pre-emptive scheduler, yielding a thread after 1ms runtime. This applies to `std::thread` and `<threads.h>`, not applications working with `OSThread` directly.

#### wut 1.0.0-beta9
###### Breaking changes
 - coreinit's `exit` is no longer defined in `<coreinit/exit.h>`. Please use `<stdlib.h>` instead, which pulls in newlib's exit.
 - RPL import sections (`.fimport_coreinit` etc.) are now garbage-collected when using wut-tools 1.1.0 or above (required). Code relying on weak links to Cafe functions may exhibit different behaviour.
 - `snd_core` and `snd_user` are no longer linked, due to naming conflicts with `sndcore2` and `snduser2`. wut has never shipped headers for these libraries, but if you are using them, please switch to `sndcore2` and `snduser2`.
 - Changes to CMake's linker flags may cause existing build trees to fail. Please delete any old build files and re-run CMake.
 - Two new symbols, `__rpx_start` and `__rpl_start`, are now used internally by the toolchain, while `_start` is now undefined. As usual, applications are strongly discouraged from prefixing any symbol with two underscores, in order to avoid conflicts of this type.

###### Deprecations
 - `WUT_ROOT` should no longer be defined in the user's environment, and will be set to `$DEVKITPRO/wut` internally. CMake lists and makefiles that use `$WUT_ROOT/share` to find `wut.mk` or `wut.toolchain.cmake` should be changed to `$DEVKITPRO/wut/share`.
 - All of wut's static libraries (`-lcoreinit`, `-lwhb`, etc.) have been merged into a single `libwut`, which gets automatically linked in for all builds. While empty static libraries have been provided for CMake builds to ease the transition, these will be removed eventually. Applications should remove the build flags to link any of wut's libraries.
 - Similarly, wut's build configuration options (devoptab, wutmalloc, newlib) are now integrated into `libwut`. For CMake builds, the `wut_enable_*` macros will now log a deprecation warning, and should be removed as soon as possible.
 - Use of `wut.mk` as a build system is now deprecated. Applications should move to `wut_rules` and devkitPro-style makefiles, such as those in [the samples](/samples/make). `wut.mk` will not be updated further, and will be removed in a future release.

###### Other changes
 - Builds refactored: wut now uses Makefiles to build itself, as well as providing a devkitPro-style `wut_rules` file - see the `samples/make` folder. The cmake samples are now in `samples/cmake`.
 - A new linking feature, `__rplwrap`, was added to help deal with conflicts between newlib's and Cafe's functions. Because of this, wut 1.0.0-beta9 requires wut-tools 1.1.0 or newer.
 - Using rplwrap, newlib's `exit` is now correctly chained with coreinit's - calls like `atexit` should work; whether calling `exit` or just returning from `main`. Applications using coreinit's `_Exit` are encouraged to migrate to a normal `exit` call.
 - A new header file, `<coreinit/codegen.h>`, has been added and documented for OSCodegen functionality.


#### wut 1.0.0-beta8
