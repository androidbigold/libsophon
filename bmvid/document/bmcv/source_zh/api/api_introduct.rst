BMCV API
===============================
简要说明BMCV API由哪一部分硬件实现

**以下接口BM1684X尚未实现:**

*  bmcv_image_canny
*  bmcv_image_dct
*  bmcv_image_draw_lines
*  bmcv_fft
*  bmcv_image_lkpyramid
*  bmcv_image_morph
*  bmcv_image_sobel

+-----+----------------------------------+-----------+-----------+
| num |         API                      |   BM1684  | BM1684X   |
+=====+==================================+===========+===========+
| 1   | bmcv_as_strided                  |NOT SUPPORT|   TPU     |
+-----+----------------------------------+-----------+-----------+
| 2   | bmcv_image_absdiff               |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 3   | bmcv_image_add_weighted          |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 4   | bmcv_base64                      |  SPACC    |  SPACC    |
+-----+----------------------------------+-----------+-----------+
| 5   | bmcv_image_bayer2rgb             |NOT SUPPORT|   TPU     |
+-----+----------------------------------+-----------+-----------+
| 6   | bmcv_image_bitwise_and           |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 7   | bmcv_image_bitwise_or            |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 8   | bmcv_image_bitwise_xor           |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 9   | bmcv_calc_hist                   |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 10  | bmcv_image_canny                 |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 11  | bmcv_image_convert_to            |   TPU     |  VPP+TPU  |
+-----+----------------------------------+-----------+-----------+
| 12  | bmcv_image_copy_to               |   TPU     |  VPP+TPU  |
+-----+----------------------------------+-----------+-----------+
| 13  | bmcv_image_dct                   |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 14  | bmcv_distance                    |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 15  | bmcv_image_draw_lines            |   CPU     |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 16  | bmcv_image_draw_rectangle        |   TPU     |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 17  | bmcv_feature_match               |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 18  | bmcv_fft                         |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 19  | bmcv_image_fill_rectangle        |   TPU     |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 20  | bmcv_image_gaussian_blur         |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 21  | bmcv_gemm                        |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 22  | bmcv_image_jpeg_enc              |   JPU     |   JPU     |
+-----+----------------------------------+-----------+-----------+
| 23  | bmcv_image_jpeg_dec              |   JPU     |   JPU     |
+-----+----------------------------------+-----------+-----------+
| 24  | bmcv_image_laplacian             |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 25  | bmcv_matmul                      |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 26  | bmcv_min_max                     |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 27  | bmcv_nms_ext                     |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 28  | bmcv_nms                         |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 29  | bmcv_image_resize                |  VPP+TPU  |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 30  | bmcv_image_sobel                 |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 31  | bmcv_sort                        |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 32  | bmcv_image_storage_convert       |  VPP+TPU  |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 33  | bmcv_image_threshold             |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 34  | bmcv_image_transpose             |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 35  | bmcv_image_vpp_basic             |   VPP     |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 36  | bmcv_image_vpp_convert_padding   |   VPP     |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 37  | bmcv_image_vpp_convert           |   VPP     |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 38  | bmcv_image_vpp_csc_matrix_convert|   VPP     |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 39  | bmcv_image_vpp_stitch            |   VPP     |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 40  | bmcv_image_warp_affine           |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 41  | bmcv_image_warp_perspective      |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 42  | bmcv_image_watermark_superpose   |NOT SUPPORT|   TPU     |
+-----+----------------------------------+-----------+-----------+
| 43  | bmcv_nms_yolo                    |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 44  | bmcv_cmulp                       |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 45  | bmcv_faiss_indexflatIP           |NOT SUPPORT|   TPU     |
+-----+----------------------------------+-----------+-----------+
| 46  | bmcv_faiss_indexflatL2           |NOT SUPPORT|   TPU     |
+-----+----------------------------------+-----------+-----------+
| 47  | bmcv_image_yuv2bgr_ext           |   TPU     |   VPP     |
+-----+----------------------------------+-----------+-----------+
| 48  | bmcv_image_yuv2hsv               |   TPU     |  VPP+TPU  |
+-----+----------------------------------+-----------+-----------+
| 49  | bmcv_batch_topk                  |   TPU     |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 50  | bmcv_image_put_text              |   CPU     |   CPU     |
+-----+----------------------------------+-----------+-----------+
| 51  | bmcv_hm_distance                 |NOT SUPPORT|   TPU     |
+-----+----------------------------------+-----------+-----------+
| 52  | bmcv_axpy                        |    TPU    |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 53  | bmcv_image_pyramid_down          |    TPU    |   TPU     |
+-----+----------------------------------+-----------+-----------+
| 54  | bmcv_image_quantify              |NOT SUPPORT|   TPU     |
+-----+----------------------------------+-----------+-----------+

**注意：**

对于BM1684和BM1684X而言，以下两个算子的实现需要结合BMCPU与Tensor Computing Processor：

+-----+----------------------------------+
| num |         API                      |
+=====+==================================+
| 1   | bmcv_image_lkpyramid             |
+-----+----------------------------------+
| 2   | bmcv_image_morph                 |
+-----+----------------------------------+

















































































