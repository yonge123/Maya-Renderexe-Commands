```python
// Render Flags
usage: Render <options> <filename>
where <filename> is a Maya ASCII or a Maya Binary file.


startFrame            -s   <float>     starting frame for an animation sequence

endFrame              -e   <float>     end frame for an animation sequence

byFrame               -b   <float>     by frame (or step)
                                       for an animation sequence

startExtension        -se  <int>       starting number for the output image
                                       frame file name extensions

byExtension           -be  <int>       by extension (or step) for the output
                                       image frame file name extension

extensionPadding      -pad <int>       number of digits in the output image
                                       frame file name extension

project               -proj <dir>      project directory to use

renderDirectory       -rd  <path>      directory in which to store image file

image                 -im  <filename>  image file output name (identical to -p)

pix                   -p   <filename>  image file output name (identical to -im)

mayaExtension         -me  <boolean>   append maya file name to image name
                                       if true

mayaFormat            -mf  <boolean>   append image file format to image name
                                       if true

cameraOverride        -cam <name>      all subsequent -im -p -ar -sa flags
                                       apply only to <camera_name>
                                       (specifying '-cam <camera_name>' enables
                                       rendering for that camera). If '-cam
                                       <camera_name>' is on the command line,
                                       then only the camera(s) specified on the
                                       command line will be rendered.

gamma                 -g   <float>     gamma value

ignoreFilmGate        -ifg <boolean>   use the film gate for rendering if false

imageHeight           -ih  <int>       height of image in pixels

imageWidth            -iw  <int>       width of image in pixels

deviceAspectRatio     -ard <float>     device aspect ratio for the rendered image

aspectRatio           -ar  <float>     aspect ratio for the film aperture

maximumMemory         -mm  <int>       renderer maximum memory use
                                       (in Megabytes)

motionBlur            -mb  <boolean>   motion blur on/off

motionBlurByFrame     -mbf <float>     motion blur by frame

shutterAngle          -sa  <float>     shutter angle for motion blur (1-360)

motionBlur2D          -mb2d <boolean>  motion blur 2D on/off

blurLength            -bll <float>     2D motion blur blur length

blurSharpness         -bls <float>     2D motion blur blur sharpness

smoothValue           -smv <int>       2D motoin blur smooth value

smoothColor           -smc <boolean>   2D motion blur smooth color on/off

keepMotionVector      -kmv <boolean>   keep motion vector for 2D motion blur on/off

useFileCache          -uf  <boolean>   use the tessellation file cache

optimizeInstances     -oi  <boolean>   dynamically detects similarly
                                       tessellated surfaces

reuseTessellations    -rut <boolean>   reuse render geometry to
                                       generate depth maps

useDisplacementBbox   -udb <boolean>   use the displacement bounding box scale to
                                       optimize displacement-map performance

enableDepthMaps       -edm <boolean>   enable depth map usage

enableRayTrace        -ert <boolean>   enable ray tracing

reflections           -rfl <int>       maximum ray-tracing reflection level

refractions           -rfr <int>       maximum ray-tracing refraction level

renderLayers          -rl <boolean|name>  render each layer separately

renderPasses          -rp <boolean|name>  render passes separately

renderSubdirs         -rs <boolean>    render layer output placed in subdirectories

shadowLevel           -sl  <int>       maximum ray-tracing shadow ray depth

edgeAntiAliasing      -eaa <quality>   The anti-aliasing quality of EAS
                                       (Abuffer). One of highest high medium low

useFilter             -ufil <boolean>  if true, use the multi-pixel filtering
                                       otherwise use single pixel filtering.

pixelFilterType       -pft  <filter>   when useFilter is true, identifies one of the
                                       following filters: box, triangle
                                       gaussian, quadraticbspline, plugin

shadingSamples        -ss  <int>       global number of shading samples
                                       per surface in a pixel

maxShadingSamples     -mss <int>       maximum number of adaptive shading
                                       samples per surface in a pixel

visibilitySamples     -mvs <int>       number of motion blur visibility samples

maxVisibilitySamples  -mvm <int>       maximum number of motion blur
                                       visibility samples

volumeSamples         -vs  <int>       global number of volume shading samples

particleSamples       -pss <int>       number of particle visibility samples

redThreshold          -rct <float>     red channel contrast threshold

greenThreshold        -gct <float>     green channel contrast threshold

blueThreshold         -bct <float>     blue channel contrast threshold

coverageThreshold     -cct <float>     pixel coverage contrast threshold
                                       (default is 1.0/8.0)

outputFormat          -of  <format>    output image file format. One of: si soft
                                       softimage, gif, rla wave wavefront, tiff
                                       tif, tiff16 tif16, sgi rgb, sgi16 rgb16
                                       alias als pix, iff tdi explore maya, jpeg
                                       jpg, eps, maya16 iff16, cineon cin fido,
                                       qtl quantel, tga targa, bmp

shadowPass            -sp <boolean>    generate shadow depth maps only

abortOnMissingTexture -amt             abort renderer when encountered missing texture

dontReplaceRendering  -rep             do not replace the rendered image if it already exists

verbose               -verbose <boolean> perform the render verbosely if on

iprFile               -ipr             create an IPR file

xResolution           -x   <int>       set X resolution of the final image

yResolution           -y   <int>       set Y resolution of the final image

xLeft                 -xl  <int>       set X sub-region left pixel boundary
                                       of the final image

xRight                -xr  <int>       set X sub-region right pixel boundary
                                       of the final image

yLow                  -yl  <int>       set Y sub-region low pixel boundary
                                       of the final image

yHigh                 -yh  <int>       set Y sub-region high pixel boundary
                                       of the final image

displayLayer          -l  <name>       one or more displayLayer names to render

numberOfProcessors    -n  <int>        number of processors to use. 0 indicates
                                       use all available.

tileWidth             -tw <int>        force the width of the tiles.  Valid valu
                                       are between 16 and 256.

tileHeight            -th <int>        force the height of the tiles.  Valid values
                                       are between 16 and 256.

                      -cont            allow renderer to continue when it hits errors

                      -keepPreImage    keep the renderings prior to post-process around
```
