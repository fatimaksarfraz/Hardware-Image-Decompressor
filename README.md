# Hardware-Image-Decompressor

This project focuses on designing and implementing a custom hardware-based image decompression system for the McMaster Image Compression revision 19 (.mic19) format. The goal is to bridge theoretical digital system design concepts with practical FPGA implementation by developing and verifying decompression circuitry in SystemVerilog.

Compressed image data (192 × 144 resolution) is transmitted from a PC to the DE2-115 FPGA development board via UART and stored in external SRAM. The custom digital system, synthesized onto the FPGA, reads the compressed data, performs step-by-step decompression, and reconstructs the raw RGB pixel data. The reconstructed image is then displayed on a monitor through a VGA controller.

The decompression pipeline includes: lossless decoding, requantization, inverse discrete cosine transform (IDCT), chroma upsampling and colour space conversion back to RGB.

Implementation details avaialble upon request.
