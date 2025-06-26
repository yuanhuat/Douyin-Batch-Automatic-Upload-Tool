# 抖音视频上传工具

<div align="center">
  <img src="static/favicon.svg" width="120" height="120" alt="抖音视频上传工具 Logo">
  <h3>抖音视频上传工具</h3>
  <p>一款高效的抖音批量视频上传、管理和编辑工具</p>
</div>

<style>
.feature-section {
  margin: 30px 0;
  padding: 20px;
  border-radius: 8px;
  background-color: #f8f9fa;
  box-shadow: 0 2px 6px rgba(0,0,0,0.05);
}

.feature-title {
  color: #ff2c55;
  font-size: 20px;
  margin-bottom: 15px;
  display: flex;
  align-items: center;
}

.feature-title i {
  margin-right: 8px;
}

.feature-content {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.feature-card {
  flex: 1 1 300px;
  padding: 15px;
  border-radius: 6px;
  background-color: white;
  box-shadow: 0 1px 3px rgba(0,0,0,0.1);
}

.feature-card h4 {
  color: #333;
  margin-top: 0;
  margin-bottom: 10px;
}

.feature-card p {
  color: #666;
  margin-bottom: 0;
}

.screenshot {
  max-width: 100%;
  border-radius: 6px;
  margin: 10px 0;
  box-shadow: 0 3px 10px rgba(0,0,0,0.1);
}

.badges {
  display: flex;
  gap: 10px;
  margin: 20px 0;
}

.badge {
  padding: 5px 10px;
  border-radius: 20px;
  font-size: 14px;
  color: white;
  background-color: #ff2c55;
}
</style>

<div class="badges">
  <span class="badge">自动化批量上传</span>
  <span class="badge">智能指纹管理</span>
  <span class="badge">代理服务器集成</span>
  <span class="badge">多账号管理</span>
</div>

## ✨ 主要功能

<div class="feature-section">
  <h3 class="feature-title"><i class="ri-key-line"></i> Cookie 管理</h3>
  <div class="feature-content">
    <div class="feature-card">
      <h4>浏览器模拟登录</h4>
      <p>点击“生成新Cookie”后，自动弹出浏览器，用户手动扫码或输入账号密码登录抖音，系统自动采集并保存Cookie。</p>
    </div>
    <div class="feature-card">
      <h4>代理支持</h4>
      <p>可为每个Cookie分配独立代理IP，防止账号关联和风控，支持代理测试和状态显示。</p>
    </div>
    <div class="feature-card">
      <h4>Cookie状态验证</h4>
      <p>一键检测Cookie是否有效，失效时高亮提示，支持批量验证和过期提醒。</p>
    </div>
  </div>

  **操作流程：**

  ```mermaid
  flowchart TD
      A[点击“生成新Cookie”] --> B[弹出浏览器窗口]
      B --> C[用户扫码/输入账号登录抖音]
      C --> D[系统自动采集Cookie]
      D --> E[为Cookie分配代理IP]
      E --> F[Cookie列表展示]
      F --> G[一键验证Cookie有效性]
      G --> H{Cookie有效?}
      H -- 是 --> I[正常使用]
      H -- 否 --> J[高亮提示/重新生成]
  ```
  - 支持多账号Cookie管理，代理分配，批量验证，过期提醒。
</div>

<div class="feature-section">
  <h3 class="feature-title"><i class="ri-movie-line"></i> 视频管理</h3>
  <div class="feature-content">
    <div class="feature-card">
      <h4>批量导入</h4>
      <p>支持ZIP、RAR、7Z压缩包批量导入视频，自动解压并保留原有文件夹结构。</p>
    </div>
    <div class="feature-card">
      <h4>文件树管理</h4>
      <p>以文件树形式展示本地视频，支持右键全选、批量操作、文件夹管理。</p>
    </div>
    <div class="feature-card">
      <h4>TXT标题支持</h4>
      <p>自动读取同名TXT文件作为视频标题和描述，提升批量上传效率。</p>
    </div>
  </div>

  **操作流程：**

  ```mermaid
  flowchart TD
      A[上传压缩包/本地视频] --> B[自动解压/扫描文件夹]
      B --> C[文件树结构展示]
      C --> D[右键全选/多选/清空选择]
      D --> E[读取同名TXT作为标题/描述]
      E --> F[已选视频列表展示]
      F --> G[准备上传/编辑]
  ```
  - 支持批量导入、结构化管理、TXT自动配对。
</div>

<div class="feature-section">
  <h3 class="feature-title"><i class="ri-upload-cloud-line"></i> 视频上传</h3>
  <div class="feature-content">
    <div class="feature-card">
      <h4>多任务队列</h4>
      <p>可为不同账号创建多个上传任务，支持任务暂停、恢复、删除。</p>
    </div>
    <div class="feature-card">
      <h4>定时发布</h4>
      <p>每个任务可设置定时发布或立即发布，支持批量定时。</p>
    </div>
    <div class="feature-card">
      <h4>自定义区域</h4>
      <p>可为每个视频选择不同地理位置，提升推荐效果。</p>
    </div>
  </div>

  **操作流程：**

  ```mermaid
  flowchart TD
      A[选择视频/账号] --> B[设置发布时间（定时/立即）]
      B --> C[选择地理位置/标签]
      C --> D[添加到上传队列]
      D --> E[任务队列管理（暂停/恢复/删除）]
      E --> F[上传进度实时显示]
      F --> G[上传完成/失败提示]
  ```
  - 支持多账号多任务，定时发布，实时进度反馈。
</div>

<div class="feature-section">
  <h3 class="feature-title"><i class="ri-settings-line"></i> 视频权限管理</h3>
  <div class="feature-content">
    <div class="feature-card">
      <h4>远程视频列表</h4>
      <p>一键获取账号下所有已上传视频，展示视频状态、发布时间、播放量等数据。</p>
    </div>
    <div class="feature-card">
      <h4>权限修改</h4>
      <p>批量修改视频公开/私密/仅好友可见等权限，支持一键全选。</p>
    </div>
    <div class="feature-card">
      <h4>视频删除</h4>
      <p>批量或单独删除已上传视频，支持进度反馈和失败重试。</p>
    </div>
  </div>

  **操作流程：**

  ```mermaid
  flowchart TD
      A[获取远程视频列表] --> B[展示视频数据（状态/播放量等）]
      B --> C[批量选择视频]
      C --> D[设置权限（公开/私密/好友）]
      C --> E[批量删除]
      D --> F[权限修改进度反馈]
      E --> G[删除进度反馈]
      F & G --> H[操作完成/失败提示]
  ```
  - 支持批量权限管理、删除、进度反馈。
</div>

<div class="feature-section">
  <h3 class="feature-title"><i class="ri-video-edit-line"></i> 视频编辑</h3>
  <div class="feature-content">
    <div class="feature-card">
      <h4>在线编辑</h4>
      <p>支持在线视频剪切、调速、添加滤镜、特效等操作，所见即所得。</p>
    </div>
    <div class="feature-card">
      <h4>视频倒放</h4>
      <p>一键生成倒放视频，适合创意内容制作。</p>
    </div>
    <div class="feature-card">
      <h4>自定义参数</h4>
      <p>支持高级FFmpeg参数，满足专业用户需求。</p>
    </div>
  </div>

  **操作流程：**

  ```mermaid
  flowchart TD
      A[选择视频] --> B[剪切/倒放/调速/滤镜/特效]
      B --> C[实时预览效果]
      C --> D[保存新视频]
      D --> E[导出/上传]
  ```
  - 支持多种编辑方式，实时预览，编辑后可直接上传。
</div>

<div class="feature-section">
  <h3 class="feature-title"><i class="ri-search-line"></i> 内容爬取</h3>
  <div class="feature-content">
    <div class="feature-card">
      <h4>视频搜索</h4>
      <p>按关键词、用户、热门榜单、链接等多种方式爬取抖音内容。</p>
    </div>
    <div class="feature-card">
      <h4>结果展示</h4>
      <p>爬取结果以表格/卡片形式展示，支持筛选、排序、批量操作。</p>
    </div>
    <div class="feature-card">
      <h4>批量下载/导出</h4>
      <p>支持一键批量下载爬取到的视频，或导出为Excel/CSV。</p>
    </div>
  </div>

  **操作流程：**

  ```mermaid
  flowchart TD
      A[输入关键词/用户/链接/热门] --> B[发起爬取请求]
      B --> C[获取内容数据]
      C --> D[表格/卡片展示结果]
      D --> E[筛选/排序/批量选择]
      E --> F[批量下载/导出]
  ```
  - 支持多种爬取方式，结果可批量下载或导出。
</div>

<div class="feature-section">
  <h3 class="feature-title"><i class="ri-download-line"></i> 视频下载</h3>
  <div class="feature-content">
    <div class="feature-card">
      <h4>批量下载</h4>
      <p>支持批量下载爬取或搜索到的视频，自动去除水印，高清保存。</p>
    </div>
    <div class="feature-card">
      <h4>下载进度</h4>
      <p>实时显示每个视频的下载进度、速度、状态。</p>
    </div>
    <div class="feature-card">
      <h4>自动导入</h4>
      <p>下载完成后自动导入到本地视频库，便于后续管理和上传。</p>
    </div>
  </div>

  **操作流程：**

  ```mermaid
  flowchart TD
      A[选择要下载的视频] --> B[批量发起下载任务]
      B --> C[实时显示进度/状态]
      C --> D[下载完成后自动导入视频库]
      D --> E[可直接管理/上传]
  ```
  - 支持批量下载、进度监控、自动导入。
</div>
