# music_player version 2.0
Web music player combine with lyric and controller.

### 待优化
- [x] 在 iOS 中 `.slider-runnable-track` 滑动卡顿；
      将 `.wrapper::after` 伪元素替换成 `<div class="wrapper-background"></div>` 后解决；
- [x] 在 Android Chrome 中 `currentTime` 错误。
      网络问题，将较大文件转移至 CDN 中即可。

### OS X Safari 中发现的问题：
- [ ] `-webkit-backdrop-filter` 属性在打开 Safari 检查器后异常，具体表现为：仅对第一个使用此属性的元素生效。