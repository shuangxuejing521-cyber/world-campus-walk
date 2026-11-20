# 投稿指南 · 기여 안내 · Contributing

## 中文

### 用什么方式建都可以

手工建模（Blender、SketchUp、3ds Max、Maya）、手机或无人机实景扫描（Polycam、Luma、RealityScan）、游戏引擎（Unity、Unreal）、Minecraft、AI 生成，或者几种混合，全由你们决定。我们只在乎最后的校园能被走进去。

### 两种参加方式

| 方式 | 适合谁 | 怎么做 |
|---|---|---|
| 表单 | 会建模、不熟悉 Git | 填“认领校园”，完成后填“提交模型”，贴上文件下载链接 |
| Pull Request | 熟悉 Git | 在 `campuses/<学校代号>/` 下放 `model.glb` 和 `campus.json` |

### 交什么文件

下面是**建议**，不是门槛。做不到的地方直接告诉我们，维护者会帮忙转换和调整。

- **格式**：最好是 GLB（glTF 2.0 二进制）；大多数软件都能导出。只能导出 FBX、OBJ、USDZ 或其他格式也可以先交
- **比例**：1 单位 = 1 米
- **方向**：Y 轴向上，北方为 −Z
- **原点**：校园中心的地面，写在 `campus.json` 的经纬度里
- **大小**：不超过 20 MB；贴图单张不超过 2048 像素
- **面数**：整座校园建议 30 万三角面以内，手机也要能跑
- **命名**：每栋建筑一个物体，用当地语言的楼名

### 内容规则

- 不使用校徽、校标等商标，除非附上学校的书面同意
- 不出现可辨认的真人、车牌或隐私信息
- 只提交自己制作、或有权使用的素材，并写明来源
- 建筑轮廓可以取自 OpenStreetMap，需保留署名

### 授权与署名

提交即表示你同意模型以 CC BY 4.0 发布。校园页面会写上团队名和成员名，`campus.json` 的 `authors` 里写谁，页面就署谁。

### 审核

维护者检查规范、能否正常加载、内容是否合规，通常一周内回复。

---

## 한국어

### 어떤 방식으로 만들어도 됩니다

직접 모델링(Blender, SketchUp, 3ds Max, Maya), 휴대폰·드론 스캔(Polycam, Luma, RealityScan), 게임 엔진(Unity, Unreal), 마인크래프트, AI 생성, 또는 여러 방식을 섞어도 좋습니다. 중요한 것은 걸어 들어갈 수 있는 캠퍼스입니다.

### 참여 방법 두 가지

| 방법 | 대상 | 절차 |
|---|---|---|
| 양식 | 모델링은 하지만 Git이 낯선 분 | ‘캠퍼스 맡기’ 작성 후, 완성되면 ‘모델 제출’에 파일 링크 첨부 |
| Pull Request | Git에 익숙한 분 | `campuses/<학교 코드>/`에 `model.glb`와 `campus.json` 추가 |

### 제출 파일

아래는 **권장 사항**이며 필수 조건이 아닙니다. 맞추기 어려운 부분은 알려 주시면 관리자가 변환과 조정을 돕습니다.

- **형식**: GLB (glTF 2.0 바이너리)가 가장 좋습니다. FBX, OBJ, USDZ 등 다른 형식도 먼저 제출해도 됩니다
- **축척**: 1단위 = 1 m
- **방향**: Y축이 위, 북쪽이 −Z
- **원점**: 캠퍼스 중심의 지면. 위도와 경도는 `campus.json`에 기록
- **크기**: 20 MB 이하, 텍스처 한 장 2048픽셀 이하
- **폴리곤**: 캠퍼스 전체 30만 삼각형 이내 권장
- **이름**: 건물마다 오브젝트 하나, 현지 언어 건물명 사용

### 내용 규칙

- 학교의 서면 동의 없이는 교표 등 상표를 쓰지 않습니다
- 식별 가능한 실제 인물, 차량 번호판, 개인 정보를 넣지 않습니다
- 직접 만들었거나 사용 권한이 있는 자료만 제출하고 출처를 밝힙니다
- 건물 윤곽은 OpenStreetMap에서 가져올 수 있으며 저작자 표시를 유지합니다

### 라이선스와 표기

제출하면 모델을 CC BY 4.0으로 공개하는 데 동의한 것으로 봅니다. `campus.json`의 `authors`에 적힌 이름이 캠퍼스 페이지에 표시됩니다.

### 검토

관리자가 규격, 로딩 여부, 내용을 확인하고 보통 일주일 안에 답합니다.

---

## English

### Build it any way you like

Hand modelling (Blender, SketchUp, 3ds Max, Maya), phone or drone scanning (Polycam, Luma, RealityScan), game engines (Unity, Unreal), Minecraft, AI tools, or a mix: it is your choice. What matters is a campus people can walk into.

### Two ways to take part

| Way | For | How |
|---|---|---|
| Forms | Modellers who do not use Git | Fill in Claim a campus, then Submit a model with a download link |
| Pull request | People comfortable with Git | Add `model.glb` and `campus.json` under `campuses/<campus-id>/` |

### What to send

These are **recommendations**, not entry requirements. Tell us where you can't meet them and a maintainer will help convert and adjust.

- **Format**: GLB (glTF 2.0 binary) is best, and most tools export it. FBX, OBJ, USDZ or other formats are fine to send first
- **Scale**: 1 unit = 1 metre
- **Orientation**: Y up, north is −Z
- **Origin**: ground level at the campus centre; its latitude and longitude go in `campus.json`
- **Size**: 20 MB or less; textures up to 2048 px
- **Triangles**: aim for under 300,000 for the whole campus so phones can run it
- **Naming**: one object per building, named in the local language

### Content rules

- No crests or other trademarks without the university's written consent
- No recognisable real people, number plates or private information
- Submit only material you made or have the right to use, and state its source
- Building footprints may come from OpenStreetMap, with attribution kept

### Licence and credit

By submitting you agree to publish the model under CC BY 4.0. The names in `authors` in `campus.json` are the names shown on the campus page.

### Review

A maintainer checks the specification, loading and content, and normally replies within a week.
