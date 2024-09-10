Build Version 24.5.0.1
Build Data 240910

///////////////////////////////////////////////////////////////////////////////////////////////////
Compatible LabVIEW Versions: >= 2024(64bit).
Software Prerequest: Vision Development Module >= 2024Q1

Optional (Install only if require support from Codec):
Codec: Chimea_Display_Codec_Setup.exe
(https://github.com/steven414/Chimera_Display_Build/releases/download/Optional/Chimera_Display_Codec_Setup.exe)

Optional (Install only if require support from OpenCV.lvlib or sklearn.lvlib):
Python Core and PIP: python-3.6.8-amd64.exe
OpenCV: pip install opencv-contrib-python==4.6.0.66
scikit-learn: pip install -U scikit-learn

///////////////////////////////////////////////////////////////////////////////////////////////////
License:
1: Run "License_Activator.exe" to get your Computer ID
2: Provide your Computer ID and receive a "License" file
3: Import and activate "Licesne" file through "License_Activator.exe" 

///////////////////////////////////////////////////////////////////////////////////////////////////
Change Log:
///////////////////////////////////////////////////////////////////////////////////////////////////
2024.09.10
1: Add support for importing Gain (Color Correction Matrix) Parameters from JSON file in "Image Processing" panel
2: Add example Color Correction Matrix JSON files in example data->Sensor_Model
3: Minor UI adjustment
///////////////////////////////////////////////////////////////////////////////////////////////////
2024.09.05
1："TDMS File Frame Extractor" now supports extracting from TDMS file with all Virtual Channel
2: Upgrade library from LabVIEW 2023 to LabVIEW 2024
3：Add new GMSL2 YUV422 with Virtual Channel TDMS example data
///////////////////////////////////////////////////////////////////////////////////////////////////
2024.04.03
1: Improve License activation process experience
2: "Get_Computer_ID.exe" now has been changed to "License_Activator.exe"
3: Improve installation process experience for Codec
4: Minor bug fix
5: Minor UI adjustment
///////////////////////////////////////////////////////////////////////////////////////////////////
2024.03.25
1: Update "Gain"(Color Correction Matrix) function in Image Processing panel
2: Minor bug fix
///////////////////////////////////////////////////////////////////////////////////////////////////
2024.03.19
1: Include absolute timestamp into snap file name for TDMS
2: Add support for snap file naming prefix
3: Add support for snap file naming configuration in Advanced Snap panel
///////////////////////////////////////////////////////////////////////////////////////////////////
2024.02.06
1: Major Update for Image_Viewer_4.0.vi
2: Add support for viewing TDMS with Virtual Channel
3: "Image_Viewer_3.0", "MIPI_LLP_Analyzer_TDMS" and "MIPI_LLP_Timestamp_Viewer" now supports TDMS with Virtual Channel
4: "TDMS_File_Frame_Extractor" now supports extracting from TDMS file based on the Virtual Channel
5: "ImageSenderShim_Timestamp_Embedded_Data_Generator" does not support TDMS with multiple Virtual Channels
///////////////////////////////////////////////////////////////////////////////////////////////////
2024.01.05
1: Add function to display RAW14 sensor data
2: Add image cropping function in Advanced Snap panel
3: Minor bug fix
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.12.20
1: Merge Image_Viewer_RAW into Image_Viewer_3.0
2: Add "Parse from .raw File" switch in Image_Viewer_3.0, enable to view RAW file recorded from ECU
3: Upgrade library from LabVIEW 2021 to LabVIEW 2023
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.06.16
1: Add "Scale by Power of 2" Property in "Image_Viewer_Payload_RAW"
2: Upgrade library from LabVIEW 2020 to LabVIEW 2021
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.05.12
1: Fix a bug for invalid H264 bitrate configuration in Codec
2: Delete quality configuration in Codec, and control video quality through CBR (constant bitrate) 
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.04.06
1: Merge "tools->TDMS_to_Payload_BIN.vi" into Image_Viewer_3.0.vi
2: In Image_Viewer_3.0, add a "Enable Advanced Snap" control to open Advanced Snap panel
3: Support snapping multiple frames' payload into a single BIN file or multiple PNG files
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.03.28
1: Minor bug fix for Codec
2: Minor bug fix for Image_Viewer_3.0.vi to handle corrupted LLP
3: Minor bug fix for Image_Viewer_3.0.vi to allow alternative snap saving folder path
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.03.16
1: Fix a bug in "tools->TDMS_File_Fixer"
2: Add support for saving specified packet payload to TDMS in "tools->MIPI_LLP_Analyzer_TDMS"
3: Add support for disable parsing TDMS "LLP Table" in "tools->MIPI_LLP_Analyzer_TDMS"
4: Add support for saving specified packet timestamp to TDMS in "tools->MIPI_LLP_Timestamp_Viewer"
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.02.27
1: Add support for analyzing I2C from "User_Timestamps.tdms"
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.02.16
1: Improve user experience for "tools->ImageSenderShim_Timestamp_Embedded_Data_Generator.vi"
2: Rewrite tools->TDMS_File_Fixer to improve efficiency
3: For TDMS files with corrupted first LLP, enable "Update Frame Start Index to File" to fix the file in "TDMS_File_Fixer"
4: In Image_Viewer_3.0, add a "Manual Overwrite Offset" control
5: Fix a bug in MIPI_LLP_Aanalyzer_TDMS.vi to support TDMS file with corrupted first LLP
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.02.10
1: Fix a bug in "Image_Viewer_3.0" INI configuration window
2: Fix a bug in "Image_Viewer_3.0" Codec window
3：Support get absoulte timestamp from TDMS Property "T0" from Group and Channel "LLP Pacaket Data"
///////////////////////////////////////////////////////////////////////////////////////////////////
2023.02.02
1: Add "tools->ImageSenderShim_Timestamp_Embedded_Data_Generator.vi"
2：Add ImageSenderShim_Timestamp_Embedded_Data_Generator.exe to build
3: ImageSenderShim_Timestamp_Embedded_Data_Generator.exe is used to generate files for NI ADAS Replay HIL from TDMS
4: Add new RAW12 TDMS example data and example corresponding .dat files
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.11.24
1: Minor bug fix
2: Change API VI to "Preallocated Clone" to increase the parallel call speed
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.11.10
1: Add "tools->MIPI_LLP_Analyzer_TDMS (GMSL1).vi"
2: Add MIPI_LLP_Analyzer_TDMS (GMSL1).exe to build->Addtional Tools
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.09.27
1: Minor UI adjustment for Image_Viewer_3.0
2: Minor bug fix for Codec
3: Add Image_Viewer_RAW.exe to build->Addtional Tools
4: Image_Viewer_RAW is used to view RAW12 sensor data captured from ECU with soft ISP disabled
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.09.08
1: Minor bug fix for Codec
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.09.06
1: Add support for H265 Encoding
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.08.29
1: Fix a bug for ineffective "Bitrate (kbps)" setting
2: Add "tools->Chimera_Display_Auto_Builder.vi"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.08.26
1: Improve decoding efficiency of RAW16, YUV422 frame
2: Add support for "Quality" parameters for Codec
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.08.25
1: Improve decoding efficiency of RAW12 frame
2: Improve accuracy of Codec preview report
3: Reduce intermediate file size from encoder
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.08.22
1: Major Update for Image_Viewer_3.0.vi
2: Add support for H264 Encoding
3: Add support for container "MP4", "MKV", "AVI" and "TS"
4: Add function to display RAW8 sensor data
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.08.09
1: Add feature to save t0 to TDMS from "tools->MIPI_LLP_Timestamp_Viewer.vi"
2: Relative t0 is saved to channel property "t0" from Channel "Timestamp"
3: Absolute t0 is saved to channel property "t0" from Channel "Absolute Timestamp"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.08.03
1: Add feature to view U8 type RAW12/16 LLP Payload as U16 type in "tools->MIPI_LLP_Analyzer_TDMS.vi" 
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.07.26
1: Add "Image_RGB_Color_Equalize.vi" to Image Processing
2: "Image_RGB_Color_Equalize.vi" can be used to tune RAW12 image color
3：Enhance display for RCCB Bayer Pattern
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.07.25
1: Minor bug fix
2: Change "tools->TDMS Timestamp Viewer.vi" to "tools->MIPI_LLP_Timestamp_Viewer.vi"
3: Add "MIPI_LLP_Timestamp_Viewer" to license product
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.07.18
1: Add "Image_TDMS->Image_Get_LLP_Timestamp_TDMS_1.vi" to get GMSL-1 LLP Packet Timestamp
2: Add "Image_TDMS->Image_Get_LLP_Timestamp_TDMS_2.vi" to get GMSL-2 LLP Packet Timestamp
3: Add "tools->TDMS Timestamp Viewer.vi"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.07.12
1: Add tools "tools->TDMS_File_Fixer.vi" to detect the possible first compelete frame offset
2: Add file read start offset to handle situation when the first LLP captured from GMSL2 is corrupted
3: File Read Start offset is supported at "Image_Viewer_2.0" and "TDMS_File_Frame_Extractor"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.07.08
1: Add tools "tools->GPIO_Analyzer_GSE.vi"
2: Add "GPIO_Analyzer_GSE" to license product
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.07.06
1: Minor bug fix
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.06.27
1: Minor Update for License Control API
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.06.16
1: Bug Fix for "Info" and "Image Processing" window shortcut
2: Snap processed image into PNG is allowed in the "Info" window
3: Reorder build folder, all Licesne Free programs are now put into "Addtional Tools"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.06.10
1: Add example "example->Image_Viewer_YUV_Batch.vi"
2: "Image_Viewer_YUV_Batch.vi" support read multiple BIN files in the same folder
3: Support BIN file extension filter
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.06.09
1: Add EXE build for "TDMS_File_Frame_Extractor"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.04.19
1: Add License Control
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.04.06
1: Add "tools->I2C_Analyzer_GSE.vi"
2: Change "tools->GMSL2_TAP_Recorded_I2C_to_Chimera.vi" to "tools->I2C_Analyzer_EAP.vi"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.03.21
1: Add support to view absolute timestamp based on "t0" file property in TDMS.
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.03.11
1: Bug fix for Getting Current Frame Data.
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.03.03
1: Minor bug fix
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.02.28
1: Bug fix for Image_Viwer_2.0.vi timestamp info.
2: Legacy GMSL-2 TDMS has been supported in Image_Viewer_2.0.vi.
3: EOL Legacy GMSL-2 TDMS support for the further new feature.
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.02.25
1: Major Update for Image_Viewer_2.0.vi
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.02.17
1: Rewrite the API to handle both TDMS and BIN file
2: Support Load and Save Configuration File in "example->Image_Viewer.vi"
3: Add "tools->BIN File Frame Extractor.vi"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.02.09
1: Add fucntion to overwrite TDMS file LLP packet in "MIPI_LLP_Analyzer_TDMS"
2: Bug fix for wrong display of total number of frames
3: Bug fix for wrong continuous Read Response in "GMSL2_TAP_Recorded_I2C_to_Chimera.vi"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.01.26
1: Optimize to reduce program size
2: Allow multiple instances of LabVIEW executable build
3: Add function to dislay Bytes per Frame
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.01.24
1: Minor bug fix
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.01.21
1: Add function to display .raw (RAW12 Type) file
2: Add "example->Image_Viewer_Payload_RAW.vi"
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.01.20
1: Add function to display YUV420 sensor data
2: I420, YV12, NV12, NV21, MIPI YUV420-8bit type is supported
///////////////////////////////////////////////////////////////////////////////////////////////////
2022.01.05
1: Add "tools->TDMS File Frame Extractor.vi"
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.12.17
1: Now "tools->MIPI_LLP_Analyzer_TDMS.vi" is updated for FlexRIO >= 21.3
2: Now "tools->TDMS_to_Payload_BIN.vi.vi" is updated for FlexRIO >= 21.3
3: Fix a bug in Error Injection VI calling
4：Fix a bug in MIPI_LLP_Analyzer_TDMS.vi Line Payload Display
5: Add build folder at application root for TDMS Viewer
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.12.01
1: CSI-2 TDMS logging structure is changed since FlexRIO 21.3
2: Use examples and tools with term "Legacy" for FlexRIO < 21.3
3: Use examples and tools without term "Legacy" for FlexRIO >= 21.3
4: Add "tools->TDMS File Converter.vi" from FlexRIO 21.3 to convert CSI-2 TDMS between "Default" and "Legacy" version
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.08.09
1: Add "Image_Viewer.lvlib->sklearn.lvlib->sklearn_Calculate_PLSRegression_Parameters.vi"
2: Add "Image_Viewer.lvlib->sklearn.lvlib->sklearn_Get_PLS_Predict_Picture.vi"
3: Add new folder at application root for camera model
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.08.04
1: Add "tools->Get_ROI_from_File.vi" for color calibration and camera model
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.07.09
1: Add function to display RAW16 sensor data
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.07.08
1: Modify "example->Image_Viewer_TDMS.vi" and "tools->GMLS2_LLP_Analyzer_TDMS.vi" to inlcude skipping initial frames function
2: Skipping initial frames to handle situation when the first frame captured from GMSL2 is corrupted
3: Add "Image_Viewer.lvlib->Image_TDMS->Image_Skip_Frame_TDMS.vi"
4: Fix a bug in displaying YUV422 data
/////////////////////////////////////////////////////////////////////////////////////////////////// 
2021.07.02
1: Now "tools->GMSL2_Packet_Viewer_TDMS.vi" has been changed to "GMLS2_LLP_Analyzer_TDMS.vi"
2: Add packet Timestamp analyzer in "GMLS2_LLP_Analyzer_TDMS.vi"
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.06.25
1: Changing Image Sensor Pattern is supported on the fly without quiting the program
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.06.18
1: Fix a major bug in displaying U8 type RAW12 frame and converting RGB888 to U8 type RAW12
2：Add "Image_Viewer.lvlib->Image_RAW12_U8_to_RAW12_U16.vi"
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.06.16
1: Rewrite the data structure to handle TDMS file with MIPI embedded data type packets
2：Add a tool "tools->GMSL2_Packet_Viewer_TDMS.vi" to inspect the specific packet line of frames in TDMS
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.06.15
1: Add Error Injection and Processing Module in "example->Image_Viewer_TDMS.vi"
2：Minor UI adjustment
///////////////////////////////////////////////////////////////////////////////////////////////////
2021.06.10
1: Add RAW (RGGB,BGGR,GBRG,GRBG,RCCB), RGB (RGB,BGR), YUV422(YUYV,UYVY,VYUY,YVYU) sensor pattern choice for display
2: Add I2C address Read response display in "tools->GMSL2_TAP_Recorded_I2C_to_Chimera.vi"
3: Minor UI adjustment
///////////////////////////////////////////////////////////////////////////////////////////////////