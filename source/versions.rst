..
  Copyright 2020 Intel Corporation


=======================
 HTML and PDF Versions
=======================

This section describes the versions that were available at time of
publication. See the `latest specification
<https://spec.oneapi.com/versions/latest/versions.html>`__ for
updates.

.. table:: oneAPI Versions Table
	   
  ========  ==========  =========
  Version   Date        View                                                                                                            
  ========  ==========  =========
  `1.0`_    09/14/2020  `HTML <https://spec.oneapi.com/versions/1.0/>`__ `PDF <https://spec.oneapi.com/versions/1.0/oneAPI-spec.pdf>`__
  `0.9`_    07/30/2020  `HTML <https://spec.oneapi.com/versions/0.9/>`__ `PDF <https://spec.oneapi.com/versions/0.9/oneAPI-spec.pdf>`__
  `0.85`_   06/29/2020  `HTML <https://spec.oneapi.com/versions/0.85/>`__ `PDF <https://spec.oneapi.com/versions/0.85/oneAPI-spec.pdf>`__
  `0.8`_    05/29/2020  `HTML <https://spec.oneapi.com/versions/0.8/>`__ `PDF <https://spec.oneapi.com/versions/0.8/oneAPI-spec.pdf>`__
  `0.7`_    03/26/2020  `HTML <https://spec.oneapi.com/versions/0.7/>`__ `PDF <https://spec.oneapi.com/versions/0.7/oneAPI-spec.pdf>`__
  `0.5`_    11/17/2019  `HTML <https://spec.oneapi.com/versions/0.5.0/>`__                                                                
  ========  ==========  =========

Release Notes
=============

1.0
---

* oneMKL

  * Continuing modifications to all oneMKL domains
  * Add oneMKL Exceptions and Error Handling

* oneDNN

  * Updated the DPC++ interoperability API
  * Added section about namespaces

* oneTBB

  * Updated the named requirements
  * Adjusted the API according to the latest product changes
  * Improved the wording and descriptions for the flow graph API
  * Cleared build warnings
  
* oneDAL
   * Extended Programming model section, added description of the generic methods and descriptors, introduced task notation
   * Extended Data Management section, introduced CSV data source, array, extended description of the tables and accessors
   * Extended description of Error handling
   * Added description of the training methods for PCA algorithm, introduced K-means initialization algorithm
   * Extended Common interface section, added description of service data types used in the interfaces of the library
   * Modified the library's namespace
  
* DPC++

  
* oneVPL

  * A lot of cleaning to remove GEN/CPU bias and implementation details.
  * New organization of structures' description.
  * New entry point function to expose by any implementation: MFXInitialize which replaces obsolete MFXInit and MFXInitEx.
  * Interface to choose and set subdevices (mfxExtDeviceAffinityMask) for execution.
  * Header files cleaned up by removing MFX_VERSION checks (ala #if MFX_VERSION > 1.26) from headers.

* oneCCL

  * Updated operation attributes description
  * Updated namings in API

0.9
---

* oneMKL

  * Continuing modifications to oneMKL Architecture, BLAS and LAPACK domains
  * Significant refactoring and updating of Sparse BLAS, VM, RNG, and DFT domains API
    descriptions and structure
  * Add Summary Statistics domain
  * Add future considerations and acknowledgment to appendices
  * Change top-level namespace to oneapi::mkl

* oneDNN

  * Added the specification for ``map_data()`` / ``unmap_data()`` methods of
    oneDNN memory objects
  * Extended element-wise algorithms and post operations
  * Added queries for peephole and projection weights for LSTM

* oneDPL

  * API updates, including namespaces
  * Added detailed descriptions for execution policies, non-standard algorithms, iterator types, etc

* oneTBB

  * Editorial review changes
  
* oneDAL

  * Updated description of the public header files and namespaces
  
* DPC++

  * Revised requirements to refer to the SYCL 2020 provisional specification where previous
    extensions have migrated to the SYCL specification directly
  * Added additional extensions
  * Added additional requirements against the SYCL 2020 provisional specification
  
* oneVPL

  * Added section to specify mandatory and optional API features
  * Reformatting of entire specification
  * Bug fixes in API definitions

* oneCCL

  * Added multi-device communication API
  * Added key-value store API
  * Extended list of collective operations

0.85
----

* oneVPL

  * High-performance video decode supporting MPEG-2, MPEG-4/H.264/AVC,
    H.265/HEVC, AV1, VP9, MJPEG;
  * High-performance video encode supporting MPEG-2, MPEG-4/H.264/AVC,
    H.265/HEVC, AV1, VP9, MJPEG;
  * Video processing for composition, alpha blending, deinterlace,
    resize, rotate, denoise, procamp, crop, detail, frame rate
    conversion, and color conversion.

* oneDNN

  * Added individual primitive definitions providing mathematical
    operation definitions and explaining details of their use
  * Expanded the programming model section explaining device
    abstraction and its interoperability with DPC++
  * Added the data model section explaining supported data types and
    memory layouts
  * Added specification for primitive attributes explaining, among
    other things, low-precision inference and bfloat16 training

0.8
---

* Level Zero

  * Updated to 0.95

* oneMKL

  * Continuing modifications to oneMKL Architecture and BLAS domain
  * Significant refactoring and updating of LAPACK domain API
    descriptions and structure.

* oneTBB

  * Significant rewrite and reorganization

* oneDAL

  * Extended description of Data Management component, added
    description of basic elements of algorithms, and error handling
    mechanism
  * Added description of namespaces and structure of the header files
  * Added specification of kNN algorithm
  * Introduced math notations section, extended glossary section

* oneDNN

  * Detailed descriptions for data model (tensor formats and data
    types), and execution models


0.7
---

* DPC++: 10 new language extensions including performance features
  like sub-groups and atomics, as well as features to allow more
  concise programs.
* oneDNN: Major restructuring of the document, with high-level
  introduction to the concepts
* Level Zero: Updated to 0.91. Open source release of driver
  implementing the specification
* oneDAL: Major restructuring of the document, with high-level
  introduction to the concepts
* oneVPL: Added support for device selection, context sharing,
  workstream presets and configurations, video processing and encoding
  APIs to easily construct a video processing pipeline.
* oneMKL: Added USM APIs. Major restructuring of document. Added
  architecture section with overview of execution model, memory model
  and API design.

0.5
---

Initial public release

