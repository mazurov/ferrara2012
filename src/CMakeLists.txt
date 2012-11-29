# Note that normally CMakeLists.txt would not be considered an
# input to the document, but in this special case of documenting
# UseLATEX.cmake the contents of this file is actually included
# in the document.
FILE(GLOB INCLUDES RELATIVE ${CMAKE_CURRENT_SOURCE_DIR} "*.inc.tex")
SET(IMAGES images/me.png
    images/hlt.png
    images/lhcb.png
    images/moore.png
    images/cpu01.png
    images/cpu02.png
    images/cpu03.png
    images/chep.png
    images/m3p.png
    images/plot_stat_mean_2p.png
    images/plot_stat_mean_3p.png
    images/plot_rerr_m3p.png
    images/splot.png
    images/bfamily.png
    images/fit.png
    images/spectr.png
    images/det.png
    images/bs.png
    images/mumu.png
    images/ups.png
    images/hlt_struct.png
    images/hlt_struct1.png
    )
ADD_LATEX_DOCUMENT(mazurov-ferrara2012.tex INPUTS ${INCLUDES} IMAGES ${IMAGES} DEFAULT_PDF)
