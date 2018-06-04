---
Description: Builds a 2D affine transformation matrix in the x-y plane. NULL arguments are treated as identity transformations.
ms.assetid: f46a307c-4566-42c8-8def-fb189116144e
title: D3DXMatrixAffineTransformation2D function
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# D3DXMatrixAffineTransformation2D function

Builds a 2D affine transformation matrix in the x-y plane. **NULL** arguments are treated as identity transformations.

## Syntax


```C++
D3DXMATRIX* D3DXMatrixAffineTransformation2D(
  _In_       D3DXMATRIX  *pOut,
  _In_       FLOAT       Scaling,
  _In_ const D3DXVECTOR2 *pRotationCenter,
  _In_       FLOAT       Rotation,
  _In_ const D3DXVECTOR2 *pTranslation
);
```



## Parameters

<dl> <dt>

*pOut* \[in\]
</dt> <dd>

Type: **[**D3DXMATRIX**](https://msdn.microsoft.com/windows/desktop/0911088b-50cf-4c4a-996e-351386fc359b)\***

Pointer to the [**D3DXMATRIX**](d3d10-d3dxmatrix.md) that is the result of the operation.

</dd> <dt>

*Scaling* \[in\]
</dt> <dd>

Type: **[**FLOAT**](https://msdn.microsoft.com/windows/desktop/4553cafc-450e-4493-a4d4-cb6e2f274d46)**

Scaling factor.

</dd> <dt>

*pRotationCenter* \[in\]
</dt> <dd>

Type: **const [**D3DXVECTOR2**](https://msdn.microsoft.com/windows/desktop/e61ec1c8-00b5-491f-8fb1-be97218f6c68)\***

Pointer to a [**D3DXVECTOR2**](d3d10-d3dxvector2.md), a point identifying the center of rotation. If this argument is **NULL**, an identity M<sub>rc</sub> matrix is applied to the formula in Remarks.

</dd> <dt>

*Rotation* \[in\]
</dt> <dd>

Type: **[**FLOAT**](https://msdn.microsoft.com/windows/desktop/4553cafc-450e-4493-a4d4-cb6e2f274d46)**

The angle of rotation.

</dd> <dt>

*pTranslation* \[in\]
</dt> <dd>

Type: **const [**D3DXVECTOR2**](https://msdn.microsoft.com/windows/desktop/e61ec1c8-00b5-491f-8fb1-be97218f6c68)\***

Pointer to a [**D3DXVECTOR2**](d3d10-d3dxvector2.md), representing the translation. If this argument is **NULL**, an identity Mₜ matrix is applied to the formula in Remarks.

</dd> </dl>

## Return value

Type: **[**D3DXMATRIX**](https://msdn.microsoft.com/windows/desktop/0911088b-50cf-4c4a-996e-351386fc359b)\***

Pointer to a D3DXMATRIX structure that is an affine transformation matrix.

## Remarks

This function calculates the affine transformation matrix with the following formula, with matrix concatenation evaluated in left-to-right order:

M<sub>out</sub> = Mₛ \* (M<sub>rc</sub>)-1 \* M<sub>r</sub> \* M<sub>rc</sub> \* Mₜ

where:

M<sub>out</sub> = output matrix (pOut)

Mₛ = scaling matrix (Scaling)

M<sub>rc</sub> = center of rotation matrix (pRotationCenter)

M<sub>r</sub> = rotation matrix (Rotation)

Mₜ = translation matrix (pTranslation)

The return value for this function is the same value returned in the pOut parameter. In this way, the D3DXMatrixAffineTransformation2D function can be used as a parameter for another function.

For 3D affine transformations, use D3DXMatrixAffineTransformation.

## Requirements



|                    |                                                                                         |
|--------------------|-----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX10Math.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3DX10.lib</dt> </dl>   |



## See also

<dl> <dt>

[Math Functions](d3d10-graphics-reference-d3dx10-functions-math.md)
</dt> </dl>

 

 



