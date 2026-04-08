# EXP-1068 Phase 2 Generation Log
**Date**: 2026-04-08
**Operator Cycle**: 793

## Seedance Generation

### Attempt 1 (v1)
- **Task ID**: cgt-20260408140837-q9ftz
- **Result**: FAIL
- **Issues**: 字幕文字出现在画面下方; 开场文件掉落有慢动作效果
- **Prompt策略**: 默认pipeline build_prompt（含asset://IDs + storyboard文本）

### Attempt 2 (v2)
- **Task ID**: (retry from pipeline)
- **Result**: QC timeout (180s超时)
- **Note**: 视频已下载但质检超时，pipeline标记为QC failure

### Attempt 3 (v3)
- **Task ID**: (retry from pipeline)
- **Result**: FAIL (but selected as best by Gemini)
- **Issues**: 陈默醒来时直视镜头; 老刘缺少自拍杆; 陈默Part5应坐实际站立
- **Selected**: ✅ Gemini从3次尝试中选择此版本为最佳

## Final Output
- **File**: final.mp4
- **Size**: 3.6MB
- **Resolution**: 720x1280 (portrait 9:16)
- **Duration**: ~15s

## Known Issues
1. **字幕问题**: Seedance持续生成硬字幕（v1），系统性问题
2. **面对镜头**: v3仍有一处直视镜头
3. **道具缺失**: 老刘的自拍杆在视频中未体现
4. **动作差异**: 部分Part动作与剧本不完全匹配

## 技术参数
- Ratio: 9:16
- Style: realistic
- Asset IDs: 陈默=asset-20260408125457-59mxj, 老刘=asset-20260408125510-nk4gh, 办公室-暗=asset-20260408125523-2zwbn, 校园操场-夏=asset-20260408125530-v84zh
