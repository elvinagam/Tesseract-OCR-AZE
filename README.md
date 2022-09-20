# Tesseract-OCR-AZE
[![Build status](https://ci.appveyor.com/api/projects/status/miah0ikfsf0j3819/branch/master?svg=true)](https://ci.appveyor.com/project/zdenop/tesseract/)
[![GitHub license](https://img.shields.io/badge/license-Apache--2.0-blue.svg)](https://raw.githubusercontent.com/tesseract-ocr/tesseract/main/LICENSE)
[![Downloads](https://img.shields.io/badge/download-all%20releases-brightgreen.svg)](https://github.com/tesseract-ocr/tesseract/releases/)
[![CodeFactor](https://www.codefactor.io/repository/github/elvinagam/tesseract-ocr-aze/badge)](https://www.codefactor.io/repository/github/elvinagam/tesseract-ocr-aze)
Tesseract on few examples, such as template matching for different languages (AZE)

Table of Contents
=================

* [Tesseract OCR](#tesseract-ocr)
   * [About](#about)
   * [Installing Tesseract](#installing-tesseract)
   * [License](#license)

## About

This package contains an **OCR engine** - `libtesseract` and a **command line program** - `tesseract`.
Tesseract 4 adds a new neural net (LSTM) based OCR engine which is focused
on line recognition, but also still supports the legacy Tesseract OCR engine of
Tesseract 3 which works by recognizing character patterns. Compatibility with
Tesseract 3 is enabled by using the Legacy OCR Engine mode (--oem 0).
It also needs [traineddata](https://tesseract-ocr.github.io/tessdoc/Data-Files.html) files which support the legacy engine, for example
those from the [tessdata](https://github.com/tesseract-ocr/tessdata) repository.

Note: Even though tested on an actual Azerbaijani example, I got the Turkish auto detection. So, I also used TUR traindata from Tesseract.
Tesseract has **unicode (UTF-8) support**, and can **recognize more than 100 languages** "out of the box".

Tesseract supports **[various image formats](https://tesseract-ocr.github.io/tessdoc/InputFormats)** including PNG, JPEG and TIFF.

Tesseract supports **various output formats**: plain text, hOCR (HTML), PDF, invisible-text-only PDF, TSV and ALTO (the last one - since version 4.1.0).

You should note that in many cases, in order to get better OCR results,
you'll need to **[improve the quality](https://tesseract-ocr.github.io/tessdoc/ImproveQuality.html) of the image** you are giving Tesseract.

Tesseract **can be trained to recognize other languages**.
See [Tesseract Training](https://tesseract-ocr.github.io/tessdoc/Training-Tesseract.html) for more information.

## Installing Tesseract

You can either [Install Tesseract via pre-built binary package](https://tesseract-ocr.github.io/tessdoc/Home.html)
or [build it from source](https://tesseract-ocr.github.io/tessdoc/Compiling.html).

## License

    The code in this repository is licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
