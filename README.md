# OCRPDF-TO-PPT

智能 PPT 编辑器 - PDF/图片转换与 AI 增强工具

## ✨ 功能

- **📄 多格式导入** - PDF、PNG、JPG、BMP 批量导入
- **🔍 OCR 识别** - 基于 PaddleOCR 的智能文字识别（支持竖排文字）
- **🎨 AI 图片编辑** - 集成 OpenAI/Gemini API
- **🖌️ 智能背景去除** - 基于 IOPaint 的涂抹擦除
- **📦 图层系统** - 支持透明度、位置调整
- **💾 项目管理** - 保存/加载项目，自动保存
- **📤 多格式导出** - PPT、PDF、图片序列

## 🚀 快速开始

### 安装

```bash
# 克隆项目
git clone https://github.com/Tansuo2021/OCRPDF-TO-PPT.git
cd OCRPDF-TO-PPT

# 安装依赖
pip install -r requirements.txt

```

### 运行

```bash
python run_ppt_editor_improved.py

# 调试模式
python run_ppt_editor_improved.py --debug
```

## 📖 使用指南

1. **导入文件**: 文件 → 导入 PDF / 导入图片
2. **OCR 识别**: OCR → 自动检测文本
3. **编辑文本**: 点击文本框选择，右侧面板调整属性
4. **AI 编辑**: AI → AI 替换，框选区域输入提示词
5. **背景去除**: 编辑 → 进入涂抹模式，标记后点击"生成背景"
6. **导出**: 文件 → 导出为 PPT / PDF / 图片

### 快捷键

| 功能 | 快捷键 |
|------|--------|
| 撤销/重做 | Ctrl+Z / Ctrl+Y |
| 复制/粘贴 | Ctrl+C / Ctrl+V |
| 保存 | Ctrl+S |
| 上/下一页 | Ctrl+Left / Ctrl+Right |

## ⚙️ 配置

创建 `ppt_editor_config.json`:

```json
{
  "ocr_device": "cpu",
  "ocr_autoload": true,
  "autosave_enabled": true,
  "ai_image_api": {
    "api_type": "openai",
    "openai": {
      "api_key": "your-api-key",
      "api_host": "https://api.openai.com/v1"
    }
  }
}
```

## 📊 技术栈

- **UI**: Tkinter
- **图像处理**: Pillow, OpenCV
- **OCR**: PaddleOCR
- **AI**: OpenAI / Gemini API
- **背景去除**: IOPaint
- **PDF**: PyMuPDF
- **PPT**: python-pptx

## 📝 更新日志

详见 [docs/CHANGELOG.md](docs/CHANGELOG.md)

## 📄 许可证

MIT License

---

*Made with ❤️ by [Tansuo2021](https://github.com/Tansuo2021)*
