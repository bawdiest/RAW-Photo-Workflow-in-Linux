# RAW Photo Workflow in Linux
1. Import RAWs from camera into temporary folder "filmroll"
''' bash
cp -r 
'''

2. Develop RAWs with your favorite RAW Developper (in my case I use RawTherapy)

3. Optional: Connect Remote Drive by SSH
''' bash
sshfs -p 22 admin@server.com:/photo /home/user/Pictures/Server
'''

4. Archive RAWs and according development files (ppt for RawTherapee)
''' bash
cp -r
'''

5. Update file catalog by creating hardlinks
''' bash
find  ~/Pictures/Server/ -name "*.CR2" -exec ln {} \;
'''
x
