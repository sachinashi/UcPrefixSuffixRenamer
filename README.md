# UcPrefixSuffixRenamer
アンリアルエンジンのアセットにプレフィックス（接頭辞）、サフィックス（接尾辞）を追加するリネーマーです。

エディタユーティリティブループリントにて実装しているため、右クリックだけで使用できます。

## 動作
![image](https://github.com/user-attachments/assets/aac88aaf-10f0-4b24-8001-8eebbca76ffe)

アセットを右クリックして Scripted Asset Actions （スクリプト化されたアセットアクション）を 表示します。
Prefix で接頭辞、Suffix で接尾辞が追加されます。

![image](https://github.com/user-attachments/assets/374faf96-b3a2-470d-9c16-30ad4fea7e81)

Texture に、一括で T_ を追加したい場合などに便利です。

![image](https://github.com/user-attachments/assets/559ab7e5-0227-4887-a517-1837863c5b0b)

アセットのリネーム例

## リネームの準拠先
以下の命名規則に準拠しています。

https://github.com/akenatsu/ue4-style-guide/blob/master/README.jp.md

ただし、今後使用頻度が縮小していく matinee や particle のようなものは除外してあります。

## 実装済一覧

Prefix（接頭辞）一覧

|Key|SourceString|
|---|--|
|AimOffset/1D|AO_|
|AnimationBlueprint|ABP_|
|AnimationComposite|AC_|
|AnimationMontage|AM_|
|BlendSpace/1D|BS_|
|LevelSequence|LS_|
|MorphTarget|MT_|
|Rig|Rig_|
|SkeletalMesh|SK_|
|Skeleton|SKEL_|
|AIController|AIC_|
|BehaviorTree|BT_|
|Blackboard|BB_|
|Decorator|BTDecorator_|
|Service|BTService_|
|Task|BTTask_|
|EnvironmentQuery|EQS_|
|Blueprint|BP_|
|BlueprintFunctionLibrary|BPFL_|
|BlueprintInterface|BPI_|
|BlueprintMacroLibrary|BPML_|
|Enumeration|E|
|Structure|F|
|TutorialBlueprint|TBP_|
|WidgetBlueprint|WBP_|
|Material|M_|
|Material(PostProcess)|PP_|
|MaterialFunction|MF_|
|MaterialInstance|MI_|
|MaterialParameterCollection|MPC_|
|SubsurfaceProfile|SP_|
|PhysicalMaterials|PM_|
|Texture|T_|
|TextureCube|TC_|
|MediaTexture|MT_|
|RenderTarget|RT_|
|CubeRenderTarget|RTC_|
|TextureLightProfile|TLP|
|ColorCurve|Curve_|
|DataTable|DT_|
|FoliageType|FT_|
|ForceFeedbackEffect|FFE_|
|LandscapeGrassType|LG_|
|LandscapeLayer|LL_|
|MediaPlayer|MP_|
|ObjectLibrary|OL_|
|SpriteSheet|SS_|
|TouchInterfaceSetup|TI_|
|PaperFlipbook|PFB_|
|Sprite|SPR_|
|SpriteAtlasGroup|SPRG_|
|TileMap|TM_|
|TileSet|TS_|
|PhysicalAsset|PHYS_|
|DialogueVoice|DV_|
|DialogueWave|DW_|
|ReverbEffect|Reverb_|
|SoundAttenuation|ATT_|
|SoundMix|Mix_|
|SoundWave|A_|
|Font|Font_|
|SlateBrush|Brush_|
|SlateWidgetStyle|Style_|
|Niagarasystem|NS_|
|NiagaraEmitter|NE_|
|NiagaraModule|NM_|

Suffix（接尾辞）一覧

|Key|SourceString|
|-------|-------|
|EnvQueryContext|Context|
|BlueprintComponet|Component|
|Decal|_Decal|
|Texture(Diffuse/Albedo/BaseColor)|_D|
|Texture(Normal)|_N|
|Texture(Roughness)|_R|
|Texture(Alpha/Opacity)|_A|
|Texture(AmbientOcclusion)|_O|
|Texture(Bump)|_B|
|Texture(Emissive)|_E|
|Texture(Mask)|_M|
|Texture(Specular)|_S|
|Texture(Metallic)|_M|
|ColorCurve|_Color|
|CurveTable|_Table|
|FloatCurve|_Float|
|VectorCurve|_Vector|
|SoundConcurrency|_SC|

