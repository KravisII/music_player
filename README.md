# music_player version 2.0
Web music player combine with lyric and controller.

### 待优化
- [x] 在 iOS 中 `.slider-runnable-track` 滑动卡顿；
      将 `.wrapper::after` 伪元素替换成 `<div class="wrapper-background"></div>` 后解决；
- [x] 在 Android Chrome 中 `currentTime` 错误；
      网络问题，将较大文件转移至 CDN 中即可。
- [x] 在 iOS 8.1 中布局错误；
      增加 CSS 前缀后解决。
- [x] 对桌面端进行布局适配；
	初步设定：左边纵栏为 `music-info`，右边上侧为 `lyric-text`，右边下侧为 `music-controller`。

### OS X Safari 中发现的问题：
- [ ] `-webkit-backdrop-filter` 属性在打开 Safari 检查器后异常，具体表现为：仅对第一个使用此属性的元素生效；
	Safari 的 bug。
- [ ] 歌词在部分浏览器中不显示。
	可能是 `transform` 未加 prefix，或 `vh` 单位在旧版本浏览器中不兼容。