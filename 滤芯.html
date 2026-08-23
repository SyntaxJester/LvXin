<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<meta name="theme-color" content="#4a90e2">
<title>汽车滤芯管理</title>
<script src="https://cdn.jsdelivr.net/npm/html5-qrcode@2.3.8/html5-qrcode.min.js"></script>
<style>
* { margin: 0; padding: 0; box-sizing: border-box; -webkit-tap-highlight-color: transparent; }
body {
  font-family: -apple-system, BlinkMacSystemFont, 'PingFang SC', 'Microsoft YaHei', sans-serif;
  background: #f5f6fa;
  color: #333;
  min-height: 100vh;
  padding-bottom: env(safe-area-inset-bottom);
}
.header {
  background: linear-gradient(135deg, #4a90e2, #357abd);
  color: #fff;
  padding: 20rpx;
  position: sticky;
  top: 0;
  z-index: 100;
  box-shadow: 0 2rpx 10rpx rgba(0,0,0,0.1);
}
.header h1 {
  font-size: 36rpx;
  font-weight: 600;
  text-align: center;
  padding: 10rpx 0;
}
.search-bar {
  display: flex;
  align-items: center;
  background: rgba(255,255,255,0.2);
  border-radius: 40rpx;
  padding: 10rpx 20rpx;
  margin: 10rpx 0;
}
.search-bar input {
  flex: 1;
  background: transparent;
  border: none;
  color: #fff;
  font-size: 28rpx;
  outline: none;
  padding: 10rpx;
}
.search-bar input::placeholder { color: rgba(255,255,255,0.7); }
.clear-btn {
  color: #fff;
  font-size: 32rpx;
  padding: 0 15rpx;
  cursor: pointer;
}
.filter-bar {
  display: flex;
  gap: 10rpx;
  padding: 10rpx 0;
  overflow-x: auto;
}
.filter-tag {
  background: rgba(255,255,255,0.3);
  color: #fff;
  padding: 8rpx 20rpx;
  border-radius: 20rpx;
  font-size: 24rpx;
  white-space: nowrap;
  cursor: pointer;
}
.filter-tag.active {
  background: #fff;
  color: #4a90e2;
}
.stats {
  padding: 15rpx 25rpx;
  color: #888;
  font-size: 24rpx;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.action-btns {
  display: flex;
  gap: 10rpx;
}
.action-btn {
  background: #fff;
  color: #4a90e2;
  border: none;
  padding: 8rpx 16rpx;
  border-radius: 20rpx;
  font-size: 22rpx;
  cursor: pointer;
}
.list {
  padding: 0 20rpx;
}
.card {
  background: #fff;
  margin: 15rpx 0;
  border-radius: 16rpx;
  padding: 25rpx;
  box-shadow: 0 2rpx 10rpx rgba(0,0,0,0.04);
  transition: transform 0.2s;
  position: relative;
}
.card:active { transform: scale(0.98); }
.card-image {
  width: 100%;
  max-height: 300rpx;
  object-fit: cover;
  border-radius: 12rpx;
  margin-bottom: 15rpx;
}
.card-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-bottom: 15rpx;
  border-bottom: 1rpx solid #f0f0f0;
  margin-bottom: 15rpx;
}
.goods-code {
  font-size: 32rpx;
  font-weight: bold;
  color: #333;
}
.car-model {
  font-size: 24rpx;
  color: #fff;
  background: #4a90e2;
  padding: 6rpx 16rpx;
  border-radius: 20rpx;
  max-width: 40%;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.info-row {
  display: flex;
  padding: 6rpx 0;
  font-size: 26rpx;
}
.label {
  color: #999;
  width: 100rpx;
  flex-shrink: 0;
}
.value {
  color: #333;
  flex: 1;
  word-break: break-all;
}
.empty {
  text-align: center;
  padding: 100rpx 40rpx;
  color: #999;
  font-size: 28rpx;
}
.empty-icon { font-size: 80rpx; margin-bottom: 20rpx; }
.fab-container {
  position: fixed;
  right: 30rpx;
  bottom: 50rpx;
  display: flex;
  flex-direction: column;
  gap: 20rpx;
  z-index: 50;
}
.fab {
  width: 100rpx;
  height: 100rpx;
  background: linear-gradient(135deg, #4a90e2, #357abd);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 6rpx 20rpx rgba(74,144,226,0.4);
  cursor: pointer;
}
.fab-icon { color: #fff; font-size: 44rpx; }
.fab-secondary {
  width: 80rpx;
  height: 80rpx;
  background: #fff;
  color: #4a90e2;
  box-shadow: 0 4rpx 15rpx rgba(0,0,0,0.15);
}
.fab-secondary .fab-icon { color: #4a90e2; font-size: 36rpx; }
/* 弹窗 */
.modal-mask {
  position: fixed;
  top: 0; left: 0; right: 0; bottom: 0;
  background: rgba(0,0,0,0.5);
  z-index: 200;
  display: none;
  align-items: center;
  justify-content: center;
}
.modal-mask.show { display: flex; }
.modal {
  background: #fff;
  width: 90%;
  max-width: 500px;
  max-height: 90vh;
  border-radius: 20rpx;
  overflow: hidden;
  display: flex;
  flex-direction: column;
}
.modal-header {
  padding: 25rpx;
  background: #4a90e2;
  color: #fff;
  font-size: 32rpx;
  font-weight: 600;
  text-align: center;
}
.modal-body {
  padding: 20rpx;
  overflow-y: auto;
  flex: 1;
}
.form-item {
  padding: 15rpx 0;
  border-bottom: 1rpx solid #f0f0f0;
}
.form-label {
  display: block;
  font-size: 26rpx;
  color: #888;
  margin-bottom: 8rpx;
}
.form-input, .form-textarea, .form-select {
  width: 100%;
  border: none;
  font-size: 30rpx;
  color: #333;
  outline: none;
  padding: 10rpx 0;
  background: transparent;
  font-family: inherit;
}
.form-textarea {
  min-height: 120rpx;
  resize: none;
}
.form-select {
  background: #f5f6fa;
  padding: 15rpx;
  border-radius: 8rpx;
}
.image-upload {
  display: flex;
  gap: 15rpx;
  margin-top: 10rpx;
}
.image-btn {
  flex: 1;
  padding: 20rpx;
  background: #f5f6fa;
  border: 2rpx dashed #ccc;
  border-radius: 12rpx;
  text-align: center;
  cursor: pointer;
  font-size: 26rpx;
  color: #666;
}
.image-btn:active { background: #e8e8e8; }
.image-preview {
  width: 100%;
  max-height: 400rpx;
  object-fit: cover;
  border-radius: 12rpx;
  margin-top: 15rpx;
}
.modal-footer {
  padding: 20rpx;
  display: flex;
  gap: 15rpx;
  border-top: 1rpx solid #f0f0f0;
}
.btn {
  flex: 1;
  height: 80rpx;
  border-radius: 40rpx;
  font-size: 28rpx;
  border: none;
  cursor: pointer;
}
.btn-save {
  background: linear-gradient(135deg, #4a90e2, #357abd);
  color: #fff;
}
.btn-cancel {
  background: #f0f2f5;
  color: #666;
}
.btn-copy {
  background: #fff;
  color: #4a90e2;
  border: 2rpx solid #4a90e2;
}
.btn-danger {
  background: #e43d33;
  color: #fff;
}
.btn-scan {
  background: #18bc37;
  color: #fff;
}
/* 扫码 */
#reader {
  width: 100%;
  margin: 20rpx 0;
}
/* Toast */
.toast {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background: rgba(0,0,0,0.8);
  color: #fff;
  padding: 20rpx 40rpx;
  border-radius: 10rpx;
  font-size: 28rpx;
  z-index: 999;
  display: none;
}
.toast.show { display: block; animation: fadeIn 0.3s; }
@keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
/* 隐藏文件输入 */
.hidden { display: none; }
</style>
</head>
<body>

<div class="header">
  <h1>🚗 汽车滤芯管理</h1>
  <div class="search-bar">
    <input type="text" id="searchInput" placeholder="🔍 搜索编码/OE码/车型/规格..." oninput="doSearch()">
    <span class="clear-btn" onclick="clearSearch()">✕</span>
  </div>
  <div class="filter-bar">
    <div class="filter-tag active" onclick="filterByType('all')">全部</div>
    <div class="filter-tag" onclick="filterByType('机油滤芯')">机油滤芯</div>
    <div class="filter-tag" onclick="filterByType('空气滤芯')">空气滤芯</div>
    <div class="filter-tag" onclick="filterByType('空调滤芯')">空调滤芯</div>
    <div class="filter-tag" onclick="filterByType('燃油滤芯')">燃油滤芯</div>
  </div>
</div>

<div class="stats">
  <span id="statsText">共 0 条记录</span>
  <div class="action-btns">
    <button class="action-btn" onclick="importData()">📥 导入</button>
    <button class="action-btn" onclick="exportData()">📤 导出</button>
  </div>
</div>

<div class="list" id="list"></div>

<div class="fab-container">
  <div class="fab fab-secondary" onclick="startScan()">
    <span class="fab-icon">📷</span>
  </div>
  <div class="fab" onclick="openModal()">
    <span class="fab-icon">➕</span>
  </div>
</div>

<!-- 编辑弹窗 -->
<div class="modal-mask" id="modal">
  <div class="modal">
    <div class="modal-header" id="modalTitle">新增滤芯</div>
    <div class="modal-body">
      <div class="form-item">
        <label class="form-label">滤芯类型</label>
        <select class="form-select" id="f_type">
          <option value="">请选择类型</option>
          <option value="机油滤芯">机油滤芯</option>
          <option value="空气滤芯">空气滤芯</option>
          <option value="空调滤芯">空调滤芯</option>
          <option value="燃油滤芯">燃油滤芯</option>
        </select>
      </div>
      <div class="form-item">
        <label class="form-label">货品编码</label>
        <input class="form-input" id="f_goods_code" placeholder="请输入货品编码">
      </div>
      <div class="form-item">
        <label class="form-label">OE码</label>
        <div style="display: flex; gap: 10rpx;">
          <input class="form-input" id="f_oe_code" placeholder="请输入OE码" style="flex: 1;">
          <button class="btn btn-scan" style="width: auto; padding: 0 20rpx;" onclick="scanOE()">扫码</button>
        </div>
      </div>
      <div class="form-item">
        <label class="form-label">车型</label>
        <input class="form-input" id="f_car_model" placeholder="请输入车型">
      </div>
      <div class="form-item">
        <label class="form-label">规格</label>
        <input class="form-input" id="f_specification" placeholder="请输入规格">
      </div>
      <div class="form-item">
        <label class="form-label">胶圈</label>
        <input class="form-input" id="f_rubber_ring" placeholder="请输入胶圈">
      </div>
      <div class="form-item">
        <label class="form-label">盒子</label>
        <input class="form-input" id="f_box_info" placeholder="请输入盒子">
      </div>
      <div class="form-item">
        <label class="form-label">备注</label>
        <textarea class="form-textarea" id="f_notes" placeholder="请输入备注"></textarea>
      </div>
      <div class="form-item">
        <label class="form-label">滤芯照片</label>
        <div class="image-upload">
          <div class="image-btn" onclick="document.getElementById('imageInput').click()">
            📷 拍照
          </div>
          <div class="image-btn" onclick="document.getElementById('imageInputAlbum').click()">
            🖼️ 相册
          </div>
        </div>
        <input type="file" id="imageInput" accept="image/*" capture="camera" class="hidden" onchange="handleImage(event)">
        <input type="file" id="imageInputAlbum" accept="image/*" class="hidden" onchange="handleImage(event)">
        <img id="imagePreview" class="image-preview" style="display: none;">
      </div>
    </div>
    <div class="modal-footer">
      <button class="btn btn-cancel" onclick="closeModal()">取消</button>
      <button class="btn btn-save" onclick="saveFilter()">💾 保存</button>
    </div>
  </div>
</div>

<!-- 详情弹窗 -->
<div class="modal-mask" id="detailModal">
  <div class="modal">
    <div class="modal-header">滤芯详情</div>
    <div class="modal-body" id="detailBody"></div>
    <div class="modal-footer">
      <button class="btn btn-danger" onclick="deleteCurrent()">🗑️ 删除</button>
      <button class="btn btn-copy" id="copyBtn" onclick="copyOE()">📋 复制OE码</button>
      <button class="btn btn-save" onclick="editCurrent()">✏️ 编辑</button>
    </div>
  </div>
</div>

<!-- 扫码弹窗 -->
<div class="modal-mask" id="scanModal">
  <div class="modal">
    <div class="modal-header">扫描二维码/条码</div>
    <div class="modal-body">
      <div id="reader"></div>
      <div style="text-align: center; color: #999; font-size: 24rpx; margin-top: 20rpx;">
        将条码/二维码放入框内，自动识别
      </div>
    </div>
    <div class="modal-footer">
      <button class="btn btn-cancel" onclick="stopScan()">关闭</button>
    </div>
  </div>
</div>

<div class="toast" id="toast"></div>

<script>
const STORAGE_KEY = 'filter_app_data_v2';
let filters = [];
let currentId = null;
let editingId = null;
let currentImage = null;
let currentFilterType = 'all';
let html5QrCode = null;

// 加载数据
function loadData() {
  try {
    const data = localStorage.getItem(STORAGE_KEY);
    filters = data ? JSON.parse(data) : [];
  } catch (e) {
    filters = [];
  }
  renderList();
}

// 保存数据
function saveData() {
  localStorage.setItem(STORAGE_KEY, JSON.stringify(filters));
}

// 渲染列表
function renderList() {
  const keyword = document.getElementById('searchInput').value.trim().toLowerCase();
  let list = filters;
  
  // 类型筛选
  if (currentFilterType !== 'all') {
    list = list.filter(item => item.type === currentFilterType);
  }
  
  // 关键字搜索
  if (keyword) {
    list = list.filter(item => {
      return (item.goods_code || '').toLowerCase().includes(keyword)
          || (item.oe_code || '').toLowerCase().includes(keyword)
          || (item.car_model || '').toLowerCase().includes(keyword)
          || (item.specification || '').toLowerCase().includes(keyword)
          || (item.rubber_ring || '').toLowerCase().includes(keyword)
          || (item.box_info || '').toLowerCase().includes(keyword)
          || (item.notes || '').toLowerCase().includes(keyword);
    });
  }
  
  const listEl = document.getElementById('list');
  document.getElementById('statsText').textContent = `共 ${list.length} 条记录`;
  
  if (list.length === 0) {
    listEl.innerHTML = `
      <div class="empty">
        <div class="empty-icon">📦</div>
        <div>${keyword || currentFilterType !== 'all' ? '没有找到匹配的记录' : '暂无数据，点击右下角 ➕ 添加'}</div>
      </div>
    `;
    return;
  }
  
  listEl.innerHTML = list.map(item => `
    <div class="card" onclick="viewDetail(${item.id})">
      ${item.image ? `<img src="${item.image}" class="card-image">` : ''}
      <div class="card-header">
        <div class="goods-code">${escapeHtml(item.goods_code || '未编码')}</div>
        ${item.car_model ? `<div class="car-model">${escapeHtml(item.car_model)}</div>` : ''}
      </div>
      ${item.type ? `<div class="info-row"><span class="label">类型：</span><span class="value">${escapeHtml(item.type)}</span></div>` : ''}
      ${item.oe_code ? `<div class="info-row"><span class="label">OE码：</span><span class="value">${escapeHtml(item.oe_code)}</span></div>` : ''}
      ${item.specification ? `<div class="info-row"><span class="label">规格：</span><span class="value">${escapeHtml(item.specification)}</span></div>` : ''}
      ${item.rubber_ring ? `<div class="info-row"><span class="label">胶圈：</span><span class="value">${escapeHtml(item.rubber_ring)}</span></div>` : ''}
    </div>
  `).join('');
}

// HTML 转义
function escapeHtml(str) {
  const div = document.createElement('div');
  div.textContent = str;
  return div.innerHTML;
}

// 搜索
function doSearch() {
  renderList();
}

function clearSearch() {
  document.getElementById('searchInput').value = '';
  renderList();
}

// 类型筛选
function filterByType(type) {
  currentFilterType = type;
  document.querySelectorAll('.filter-tag').forEach(tag => {
    tag.classList.remove('active');
  });
  event.target.classList.add('active');
  renderList();
}

// 打开新增弹窗
function openModal() {
  editingId = null;
  currentImage = null;
  document.getElementById('modalTitle').textContent = '新增滤芯';
  ['type', 'goods_code', 'oe_code', 'car_model', 'specification', 'rubber_ring', 'box_info', 'notes'].forEach(key => {
    document.getElementById('f_' + key).value = '';
  });
  document.getElementById('imagePreview').style.display = 'none';
  document.getElementById('modal').classList.add('show');
}

// 关闭弹窗
function closeModal() {
  document.getElementById('modal').classList.remove('show');
  document.getElementById('detailModal').classList.remove('show');
}

// 处理图片
function handleImage(event) {
  const file = event.target.files[0];
  if (!file) return;
  
  const reader = new FileReader();
  reader.onload = function(e) {
    currentImage = e.target.result;
    const preview = document.getElementById('imagePreview');
    preview.src = currentImage;
    preview.style.display = 'block';
  };
  reader.readAsDataURL(file);
}

// 保存
function saveFilter() {
  const data = {
    type: document.getElementById('f_type').value,
    goods_code: document.getElementById('f_goods_code').value.trim(),
    oe_code: document.getElementById('f_oe_code').value.trim(),
    car_model: document.getElementById('f_car_model').value.trim(),
    specification: document.getElementById('f_specification').value.trim(),
    rubber_ring: document.getElementById('f_rubber_ring').value.trim(),
    box_info: document.getElementById('f_box_info').value.trim(),
    notes: document.getElementById('f_notes').value.trim(),
    image: currentImage
  };
  
  if (!data.goods_code && !data.oe_code && !data.car_model) {
    showToast('请至少填写一项');
    return;
  }
  
  if (editingId) {
    const idx = filters.findIndex(x => x.id === editingId);
    if (idx >= 0) {
      filters[idx] = { ...filters[idx], ...data, updated_at: new Date().toISOString() };
    }
  } else {
    data.id = Date.now();
    data.created_at = new Date().toISOString();
    filters.unshift(data);
  }
  
  saveData();
  closeModal();
  renderList();
  showToast('保存成功 ✓');
}

// 查看详情
function viewDetail(id) {
  const item = filters.find(x => x.id === id);
  if (!item) return;
  currentId = id;
  
  const fields = [
    ['类型', item.type],
    ['货品编码', item.goods_code],
    ['OE码', item.oe_code],
    ['车型', item.car_model],
    ['规格', item.specification],
    ['胶圈', item.rubber_ring],
    ['盒子', item.box_info],
    ['备注', item.notes]
  ];
  
  let html = '';
  if (item.image) {
    html += `<img src="${item.image}" style="width: 100%; border-radius: 12rpx; margin-bottom: 20rpx;">`;
  }
  html += fields
    .filter(([, v]) => v)
    .map(([k, v]) => `<div class="info-row"><span class="label">${k}：</span><span class="value">${escapeHtml(v)}</span></div>`)
    .join('');
  
  document.getElementById('detailBody').innerHTML = html;
  document.getElementById('copyBtn').style.display = item.oe_code ? '' : 'none';
  document.getElementById('detailModal').classList.add('show');
}

// 编辑当前
function editCurrent() {
  const item = filters.find(x => x.id === currentId);
  if (!item) return;
  editingId = currentId;
  currentImage = item.image;
  document.getElementById('modalTitle').textContent = '编辑滤芯';
  ['type', 'goods_code', 'oe_code', 'car_model', 'specification', 'rubber_ring', 'box_info', 'notes'].forEach(key => {
    document.getElementById('f_' + key).value = item[key] || '';
  });
  
  const preview = document.getElementById('imagePreview');
  if (item.image) {
    preview.src = item.image;
    preview.style.display = 'block';
  } else {
    preview.style.display = 'none';
  }
  
  document.getElementById('detailModal').classList.remove('show');
  document.getElementById('modal').classList.add('show');
}

// 删除当前
function deleteCurrent() {
  if (!confirm('确定要删除这条记录吗？')) return;
  filters = filters.filter(x => x.id !== currentId);
  saveData();
  closeModal();
  renderList();
  showToast('已删除');
}

// 复制 OE 码
function copyOE() {
  const item = filters.find(x => x.id === currentId);
  if (!item || !item.oe_code) return;
  
  if (navigator.clipboard) {
    navigator.clipboard.writeText(item.oe_code).then(() => {
      showToast('已复制 OE码');
    });
  } else {
    const input = document.createElement('input');
    input.value = item.oe_code;
    document.body.appendChild(input);
    input.select();
    document.execCommand('copy');
    document.body.removeChild(input);
    showToast('已复制 OE码');
  }
}

// 导出数据
function exportData() {
  if (filters.length === 0) {
    showToast('暂无数据可导出');
    return;
  }
  
  const headers = ['类型', '货品编码', 'OE码', '车型', '规格', '胶圈', '盒子', '备注', '图片', '创建时间'];
  const rows = filters.map(f => [
    f.type || '', f.goods_code || '', f.oe_code || '', f.car_model || '',
    f.specification || '', f.rubber_ring || '', f.box_info || '',
    f.notes || '', f.image || '', f.created_at || ''
  ]);
  
  let csv = '\uFEFF' + headers.join(',') + '\n';
  rows.forEach(row => {
    csv += row.map(cell => `"${(cell + '').replace(/"/g, '""')}"`).join(',') + '\n';
  });
  
  const blob = new Blob([csv], { type: 'text/csv;charset=utf-8' });
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url;
  a.download = `滤芯数据_${new Date().toISOString().slice(0,10)}.csv`;
  a.click();
  URL.revokeObjectURL(url);
  showToast('导出成功');
}

// 导入数据
function importData() {
  const input = document.createElement('input');
  input.type = 'file';
  input.accept = '.csv';
  input.onchange = function(e) {
    const file = e.target.files[0];
    if (!file) return;
    
    const reader = new FileReader();
    reader.onload = function(e) {
      try {
        const text = e.target.result;
        const lines = text.split('\n').filter(line => line.trim());
        if (lines.length < 2) {
          showToast('文件格式错误');
          return;
        }
        
        const headers = lines[0].split(',').map(h => h.replace(/"/g, '').trim());
        const newFilters = [];
        
        for (let i = 1; i < lines.length; i++) {
          const values = lines[i].match(/(".*?"|[^,]+)(?=\s*,|\s*$)/g) || [];
          const cleanValues = values.map(v => v.replace(/^"|"$/g, '').replace(/""/g, '"'));
          
          const item = {
            id: Date.now() + i,
            type: cleanValues[0] || '',
            goods_code: cleanValues[1] || '',
            oe_code: cleanValues[2] || '',
            car_model: cleanValues[3] || '',
            specification: cleanValues[4] || '',
            rubber_ring: cleanValues[5] || '',
            box_info: cleanValues[6] || '',
            notes: cleanValues[7] || '',
            image: cleanValues[8] || '',
            created_at: cleanValues[9] || new Date().toISOString()
          };
          
          if (item.goods_code || item.oe_code || item.car_model) {
            newFilters.push(item);
          }
        }
        
        if (confirm(`发现 ${newFilters.length} 条记录，是否导入？\n（会与现有数据合并）`)) {
          filters = [...newFilters, ...filters];
          saveData();
          renderList();
          showToast('导入成功');
        }
      } catch (err) {
        showToast('导入失败：' + err.message);
      }
    };
    reader.readAsText(file, 'UTF-8');
  };
  input.click();
}

// 扫码功能
function startScan() {
  document.getElementById('scanModal').classList.add('show');
  
  html5QrCode = new Html5Qrcode("reader");
  const config = { fps: 10, qrbox: { width: 250, height: 250 } };
  
  html5QrCode.start(
    { facingMode: "environment" },
    config,
    (decodedText) => {
      document.getElementById('f_oe_code').value = decodedText;
      stopScan();
      showToast('扫码成功');
    },
    (errorMessage) => {}
  ).catch(err => {
    showToast('无法启动摄像头：' + err);
    stopScan();
  });
}

function stopScan() {
  if (html5QrCode) {
    html5QrCode.stop().then(() => {
      html5QrCode.clear();
      html5QrCode = null;
    });
  }
  document.getElementById('scanModal').classList.remove('show');
}

function scanOE() {
  startScan();
}

// Toast 提示
function showToast(msg) {
  const toast = document.getElementById('toast');
  toast.textContent = msg;
  toast.classList.add('show');
  setTimeout(() => toast.classList.remove('show'), 2000);
}

// 初始化
loadData();
</script>

</body>
</html>