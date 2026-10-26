libmpv for the Paattu Windows app

libmpv-2.dll  mpv's library with FFmpeg, unchanged from shinchiro's build
              mpv-dev-x86_64-20261017-git-dde0671072.7z
              https://github.com/shinchiro/mpv-winbuild-cmake/releases/tag/20261017
              (archive SHA-256 d6638b2b40561e6071627f39ad60a38e15721dc87a49f244b897911ea2edfd9f).
              Built from mpv commit dde0671072 (https://github.com/mpv-player/mpv) and the
              FFmpeg and libraries listed in https://github.com/shinchiro/mpv-winbuild-cmake
              (packages/), whose source that build script fetches. mpv and FFmpeg are under
              the GPL / LGPL: see https://github.com/mpv-player/mpv/blob/master/Copyright.
vulkan-1.dll  the Khronos Vulkan loader 1.3.296.0 (LunarG VulkanRT components),
              Apache-2.0 (vulkan-1-LICENSE.txt); libmpv-2.dll needs it to load.

Paattu ships this instead of media_kit's libmpv because that one has only
FFmpeg's equalizer audio filter, and the surround needs extrastereo.
