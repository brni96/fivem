vars = {
	"citidev_root": "http://tohjo.eu/citidev"
}

deps = {
	"vendor/luajit": Var("citidev_root") + "/luajit.git",
	"build/premake": "http://github.com/premake/premake-core.git",
	"vendor/jitasm": "http://jitasm.googlecode.com/svn/trunk/",
	"vendor/yaml-cpp": "https://github.com/jbeder/yaml-cpp.git",
	"vendor/msgpack-c": "https://github.com/msgpack/msgpack-c.git",
	"vendor/zlib": "https://github.com/madler/zlib.git",
	"vendor/gmock": "http://googlemock.googlecode.com/svn/trunk/",
	"vendor/gtest": "http://googletest.googlecode.com/svn/trunk/",
	"vendor/protobuf": "https://github.com/google/protobuf.git@5eb73dfcce20bdfe421620cb31b7b98a0c5eec88",
	"vendor/libopus": "git://git.opus-codec.org/opus.git",
	"vendor/pash": "http://tohjo.eu/citidev/pash.git",
	"vendor/breakpad": "http://google-breakpad.googlecode.com/svn/trunk/",
	"vendor/udis86": "https://github.com/vmt/udis86.git",
	"vendor/tinyxml2": "https://github.com/leethomason/tinyxml2.git",
	"vendor/cpp-uri": "https://github.com/cpp-netlib/uri.git",
	"vendor/picohttpparser": "https://github.com/h2o/picohttpparser.git@98bcc1c3b431d05d4584af66082da48e4638a675",
	"vendor/libssh": "http://tohjo.eu/citidev/libssh.git",
	"vendor/xz": "http://git.tukaani.org/xz.git",
	"vendor/curl": "https://github.com/bagder/curl.git",
	"vendor/libuv": "https://github.com/libuv/libuv.git@v1.x"
}

hooks = [
	{
		"name": "gen_udis_script",
		"pattern": "vendor/udis86/",
		"action": [ "citizenmp\prebuild_udis86.cmd" ]
	},
	{
		"name": "build_premake_win",
		"pattern": "build/premake/",
		"action": [ "citizenmp\prebuild_premake.cmd" ]
	},
	{
		"name": "build_luajit_win",
		"pattern": "vendor/luajit/src/",
		"action": [ "citizenmp\prebuild_luajit.cmd" ]
	}
]
