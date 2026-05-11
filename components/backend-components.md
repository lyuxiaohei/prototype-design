# 后台组件规范

适用于：素材库、页面装修、订单管理（运营侧）、售后审批等PC端运营工具。

#### 按钮样式

```css
.btn {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 8px 16px;
  border-radius: 6px;
  font-size: 14px;
  cursor: pointer;
  transition: all 0.3s;
  border: 1px solid #d9d9d9;
  background: #fff;
  color: #333;
}
.btn:hover { border-color: #1890ff; color: #1890ff; }
.btn-primary { background: #1890ff; border-color: #1890ff; color: #fff; }
.btn-danger { color: #ff4d4f; border-color: #ff4d4f; }
```

```html
<button class="btn btn-primary">确认</button>
<button class="btn">取消</button>
<button class="btn btn-danger">删除</button>
```

#### 素材网格

```css
.material-grid { display: grid; grid-template-columns: repeat(5, 1fr); gap: 16px; }
.material-card { border-radius: 8px; overflow: hidden; }
.card-thumbnail { height: 100px; object-fit: cover; }
```

**重要：** 5列固定布局，100px固定高度。

#### 分页组件

```css
.page-btn { min-width: 36px; height: 36px; border-radius: 6px; }
.page-btn.active { background: #1890ff; color: #fff; }
```

#### 分类树

```css
.category-panel { width: 220px; }
.category-item { padding: 8px 16px; cursor: pointer; }
.category-item.active { background: #e6f7ff; color: #1890ff; }
```
