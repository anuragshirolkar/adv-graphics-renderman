shader=/opt/pixar/RenderManProServer-20.6/bin/shader
prman=/opt/pixar/RenderManProServer-20.6/bin/prman -progress 
all:r2d2.rib scene.rib  r2d2body.slo metal.slo
	$(prman) scene.rib

r2d2body.slo: r2d2body.sl 
	$(shader) r2d2body.sl
metal.slo: metal.sl
	$(shader) metal.sl

clean:
	rm -rf *.slo *.ptc