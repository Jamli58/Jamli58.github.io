---
layout: page
title: "Curriculum Vitae"
permalink: /cv/
---

<style>
.pdf-container {
  width: 100%;
  height: 85vh;
  border: 1px solid #ddd;
  border-radius: 5px;
  overflow: hidden;
  position: relative;
}

.pdf-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
  background: transparent;
}

/* 禁用选择和右键 */
.pdf-container {
  user-select: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
}
</style>

<div class="pdf-container" oncontextmenu="return false;">
  <div class="pdf-overlay"></div>
  <iframe 
    src="{{ site.baseurl }}/files/CV_LiJian.pdf#toolbar=0&navpanes=0&scrollbar=1" 
    width="100%" 
    height="100%"
    style="border: none;">
  </iframe>
</div>

<script>
// 禁用键盘快捷键
document.addEventListener('keydown', function(e) {
  if (e.ctrlKey && (e.key === 's' || e.key === 'p')) {
    e.preventDefault();
    alert('This document is protected.');
    return false;
  }
});
</script>