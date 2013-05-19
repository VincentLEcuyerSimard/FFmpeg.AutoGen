##FFmpeg.AutoGen

Auto Generated FFmpeg wrapper for C#/.NET and Mono.  
Wrapper generated for FFmpeg 1.2.  

##Usage

Example of usage video decoding with frame extraction included in FFmpeg.AutoGen.Example project.

- on Windows:  
Put FFmpeg binaries next to application.
They can be downloaded from [Zeranoe FFmpeg builds](http://ffmpeg.zeranoe.com/builds/) for 
[32-bit](http://ffmpeg.zeranoe.com/builds/win32/shared/ffmpeg-1.2-win32-shared.7z) or
[64-bit](http://ffmpeg.zeranoe.com/builds/win64/shared/ffmpeg-1.2-win64-shared.7z).
Please note that version number should be stripped out from the file name i.e. ```avcodec-54.dll``` should be renamed or symlinked to ```avcodec.dll```. 

- on OS X:  
Install FFmpeg via [MacPorts](http://www.macports.org):
```bash
sudo port install ffmpeg +universal
```
Before run application it is necessary set enviroment variable variable ```LD_LIBRARY_PATH``` to ```/opt/local/lib``` (default MacPorts libraries location)

- on Linux:  
*todo*

##Download

Compiled wrapper:
http://sourceforge.net/projects/ffmpeg-autogen/files/

##Generation

Wrapper generator uses customized version of ctypesgencore package based on ctypesgen 0.r125.

Prerequisites:
 - Python 2.7
   with packages:
    - ctypes 1.0.2

 - gcc
   OS dependent:
    - on OS X - XCode Command Line Tools
    - on Windows - [MinGW](http://www.mingw.org)

Steps:
- Execute: python generate.py
- File "./FFmpeg.AutoGen/FFmpegInvoke.cs" will regenerated.

##License

GNU Lesser General Public License (LGPL) version 3 or later.  
http://www.gnu.org/licenses/lgpl.html

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.