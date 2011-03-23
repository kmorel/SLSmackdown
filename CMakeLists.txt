project(SLSmackdown NONE)

cmake_minimum_required(VERSION 2.8)

include(UseLATEX.cmake)

set(images
  images/TransparentOutput.png
  images/OpaqueOutput.png
  images/AccumulativeCompositeOrder.pdf
  images/TreeCompositeOrder.pdf
  images/IceTCompositeImprovements0256.pdf
  images/IceTCompositeImprovements2048.pdf
  )

add_latex_document(SLSmackdown.tex
  BIBFILES SLSmackdown.bib
  IMAGES ${images}
  )
