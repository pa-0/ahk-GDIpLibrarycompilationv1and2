# AHK GDI+ library compilation.
This is a compilation of user contributed functions for the GDIp library wrapper 
made by Tariq Porter [tic] that never made into it.

This repository is a fork of https://github.com/mmikeww/AHKv2-Gdip/ .
Unfortunately, some of the newly added functions are likely not
AHK v2 compatible, however I updated several functions to better
suit to it.

# History
- @tic created the original [Gdip.ahk](https://github.com/tariqporter/Gdip/) library
- @Rseding91 updated it to make it compatible with unicode and x64 AHK versions and renamed the file `Gdip_All.ahk`
- @mmikeww's repository updates @Rseding91's `Gdip_All.ahk` to make it compatible with AHK v2 and also fixes some bugs
- this repository attempts to gather all the GDI+ functions contributed by various people that were missing

# Comparisions

The following list is comparing Gdip_All.ahk
by Tariq Porter and Rseding91 modifications
with this new version.

## 16 MODIFIED FUNCTIONS:
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


## 68 NEW FUNCTIONS:

- Unknown source [probably mmikeww]:
  - Gdip_BitmapFromBase64()
  - GetIconDimensions()     

- by Tariq Porter [tic]:
  - Gdip_FillRoundedRectangle2()
  - Gdip_DrawRoundedRectangle2()

- by DevX and Rabiator:
  - Gdip_DrawRoundedLine()

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
  - Gdip_StartPathFigure()
  - Gdip_ClosePathFigure()
  - Gdip_DrawPath()
  - Gdip_WidenPath()
  - Gdip_ClonePath()

- By "Just Me":
  - Gdip_PathGradientCreateFromPath()
  - Gdip_PathGradientSetCenterPoint()
  - Gdip_PathGradientSetCenterColor()
  - Gdip_PathGradientSetSurroundColors()
  - Gdip_PathGradientSetSigmaBlend()
  - Gdip_PathGradientSetLinearBlend()
  - Gdip_PathGradientSetFocusScales()
  - Gdip_AddPathGradient()
  - Gdip_GetPropertyCount()
  - Gdip_GetPropertyIdList()
  - Gdip_GetPropertyItem()
  - Gdip_GetAllPropertyItems()
  - Gdip_GetPropertyTagName()
  - Gdip_GetPropertyTagType()
  - Gdip_GetPropertyItemValue()
  - GetMonitorCount
  - GetMonitorInfo
  - GetPrimaryMonitor
  - Multiple Display Monitors Functions by "Just me":
    - MDMF_Enum
    - MDMF_EnumProc
    - MDMF_FromHWND
    - MDMF_FromPoint
    - MDMF_FromRect
    - MDMF_GetInfo

- By Marius Șucan [robodesign]:
  - *Gdip_GetHistogram()
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
  - Gdip_PixelateBitmap() seems to not work.
  - awaiting pull requests for bug fixes or to have it entirely compatible with AHK v2 as well, for the newly added functions,
