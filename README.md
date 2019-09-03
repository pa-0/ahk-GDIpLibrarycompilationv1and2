# AHK GDI+ library compilation.
This is a compilation of user contributed functions for the GDI+ library wrapper made by Tariq Porter [tic] that never made it into.

This repository is a fork of https://github.com/mmikeww/AHKv2-Gdip/ . Some of the newly added functions are possibly not AHK v2 compatible.

The Tutorials/Examples are left untouched. They are the same as in the repository of @mmikeww. I added several new examples that showcase the newly supported GDI+ APIs. These are example scripts initially provided by those that coded the new functions.

# History
- @tic created the original [Gdip.ahk](https://github.com/tariqporter/Gdip/) library
- @Rseding91 updated it to make it compatible with unicode and x64 AHK versions and renamed the file `Gdip_All.ahk`
- @mmikeww's repository updates @Rseding91's `Gdip_All.ahk` to make it compatible with AHK v2 and also fixes some bugs
- this repository attempts to gather all the GDI+ functions contributed by various people that were missing

# Comparisions

The following list is comparing Gdip_All.ahk by Tariq Porter and Rseding91 modifications with this new version.

## 17 MODIFIED FUNCTIONS:
- Gdip_CreateBitmapFromClipboard()
- Gdip_SetBitmapToClipboard()
- UpdateLayeredWindow()
- SetImage()
- SetSysColorToControl()
- Gdip_BitmapFromScreen()
- Gdip_BitmapFromHWND()
- Gdip_BitmapFromBRA()
- Gdip_DrawLines()
- Gdip_FillPolygon()
- Gdip_DrawImagePointsRect()
- Gdip_SetImageAttributesColorMatrix()
- Gdip_SaveBitmapToFile()
- Gdip_CreateBitmapFromFile()
- Gdip_TextToGraphics()
- Gdip_GetClipRegion()
- Gdip_CreateTextureBrush()


## 106 NEW FUNCTIONS:

- Unknown source [probably mmikeww]:
  - Gdip_BitmapFromBase64()
  - GetIconDimensions()     

- by Tariq Porter [tic]:
  - Gdip_FillRoundedRectangle2()
  - Gdip_DrawRoundedRectangle2()

- by DevX and Rabiator:
  - Gdip_DrawRoundedLine()

- by SBC:
  - Gdip_GetImageFramesCount()

- By RazorHalo:
  - RotateAtCenter()
  - Gdip_ResetMatrix()
  - Gdip_RotateMatrix()
  - Gdip_GetPathWorldBounds()
  - Gdip_ScaleMatrix()
  - Gdip_TranslateMatrix()
  - Gdip_TransformPath()
  - Gdip_SetMatrixElements()
  - Gdip_IsVisiblePathPoint()

- By "Learning one":
  - Gdip_AddPathBeziers()
  - Gdip_AddPathBezier()
  - Gdip_AddPathLines()
  - Gdip_AddPathLine()
  - Gdip_AddPathArc()
  - Gdip_AddPathPie()
  - Gdip_SetPathFillMode()
  - Gdip_StartPathFigure()
  - Gdip_ClosePathFigure()
  - Gdip_DrawPath()
  - Gdip_WidenPath()
  - Gdip_ClonePath()
  - Gdip_CombineRegionRegion()
  - Gdip_CreateRegionPath()

- By "Just Me":
  - Gdip_PathGradientCreateFromPath()
  - Gdip_PathGradientSetCenterPoint()
  - Gdip_PathGradientSetCenterColor()
  - Gdip_PathGradientSetSurroundColors()
  - Gdip_PathGradientSetSigmaBlend()
  - Gdip_PathGradientSetLinearBlend()
  - Gdip_PathGradientSetFocusScales()
  - Gdip_AddPathGradient()
  - Gdip_LoadImageFromFile()
  - Gdip_GetPropertyCount()
  - Gdip_GetPropertyIdList()
  - Gdip_GetPropertyItem()
  - Gdip_GetAllPropertyItems()
  - Gdip_GetPropertyTagName()
  - Gdip_GetPropertyTagType()
  - Gdip_GetPropertyItemValue()
  - Multiple Display Monitors Functions by "Just me":
    - GetMonitorCount
    - GetMonitorInfo
    - GetPrimaryMonitor
    - MDMF_Enum
    - MDMF_FromHWND
    - MDMF_FromPoint
    - MDMF_FromRect
    - MDMF_GetInfo

- By Marius Șucan [robodesign]:
  - *Gdip_GetHistogram()
  - Gdip_CreateRegionRect()
  - Gdip_GetWorldTransform()
  - Gdip_CloneRegion()
  - Gdip_SetTextureWrapMode()
  - Gdip_GetTextureWrapMode()
  - Gdip_ScaleTextureTransform()
  - Gdip_RotateTextureTransform()
  - Gdip_ResetTextureTransform()
  - Gdip_ResetTextureTransform()
  - Gdip_TranslateRegion()
  - Gdip_TranslateClip()
  - Gdip_IsEmptyRegion()
  - Gdip_IsEqualRegion()
  - Gdip_IsInfiniteRegion()
  - Gdip_IsVisibleRegionPoint()
  - Gdip_IsVisibleRegionRect()
  - Gdip_SetEmptyRegion()
  - Gdip_SetInfiniteRegion()
  - Gdip_GetRegionBounds()
  - Gdip_GraphicsFlush()
  - Gdip_GetImageBounds()
  - Gdip_GetImageDimension()
  - Gdip_CloneBitmap()
  - Gdip_SetCompositingQuality()
  - Gdip_SetPageScale()
  - Gdip_SetPageUnit()
  - Gdip_SetPixelOffsetMode()
  - Gdip_SetRenderingOrigin()
  - Gdip_SetTextContrast()
  - Gdip_GetCompositingMode()
  - Gdip_GetCompositingQuality()
  - Gdip_GetInterpolationMode()
  - Gdip_GetPageScale()
  - Gdip_GetPageUnit()
  - Gdip_GetPixelOffsetMode()
  - Gdip_GetRenderingOrigin()
  - Gdip_GetTextRenderingHint()
  - Gdip_CreateDIBitmap()
  - Gdip_GetDIBits()
  - Gdip_DrawImageFX()
  - Gdip_ApplyEffect()
  - Gdip_CreateEffect()
  - Gdip_DisposeEffect()
  - GenerateColorMatrix()

(*) mainly written by swagfag, but at my request and modified it further

- By nnnik [extracted from his GDI+ class]:
  - Gdip_DrawBeziers()
  - Gdip_SetLineColors()
  - Gdip_GetLineColors()
  - Gdip_SetSolidFillColor()
  - Gdip_GetSolidFillColor()
  - Gdip_ClonePen()
  - Gdip_SetPenWidth()
  - Gdip_GetPenWidth()
  - Gdip_SetPenColor()
  - Gdip_GetPenColor()
  - Gdip_SetPenBrushFill()
  - Gdip_CreateFontFromDC()

## NOTES:
  - GetProperty() functions yield incorrect results for some meta-data/properties.
  - Gdip_PixelateBitmap() seems to not work for me [in any GDI+ library edition].
  - the newly added examples are not AHK v2 compatible
  - all other tutorials / examples throw an error on script exit on AHK v2 a104; the same applies to @mmikeww's edition
  - awaiting pull requests for bug fixes
