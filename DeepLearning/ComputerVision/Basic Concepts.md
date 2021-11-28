# Basic Concepts

## Bounding Boxes/BBoxes

表示物体位置的矩形框，通常用中心点坐标+长宽或者左上+右下坐标表示其位置和大小

## Anchor Boxes

预先设定好比例的候选框的集合，用于在其基础上回归出真实框的位置和大小

## Intersection over Union (IoU)

交并比

$$J(\mathcal{A},\mathcal{B}) = \frac{\left|\mathcal{A} \cap \mathcal{B}\right|}{\left| \mathcal{A} \cup \mathcal{B}\right|}.$$

![交并比](../../Resource/Pictures/iou.svg)

## Non-Maximum Suppresion (NMS)

非极大值抑制，在输出结果阶段，针对某个目标可能会有大量重叠的预测框，根据NMS

## 子特征图

自己定义，为描述方便，定义经过RoI Pooling 或 Aligning的feature map 为子特征图