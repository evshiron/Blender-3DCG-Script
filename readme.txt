Blender 3DCG script

���T�v
����̓I�[�v���\�[�X��3D�\�t�g�E�F�A�ł��� Blender ����3D�J�X�^��������
3D���f���t�@�C��(.tso)�̓��o�́A�|�[�Y�E���[�V�����t�@�C��(.tmo)�̓��o�͂�
�s�� Python �X�N���v�g�ł��B


���t�@�C���\��

	Python\3dcg_tso_import.py      tso�t�@�C���C���|�[�g�pPython�X�N���v�g
	Python\3dcg_tso_export.py      tso�t�@�C���G�N�X�|�[�g�pPython�X�N���v�g
	Python\3dcg_tmo_import.py      tso�t�@�C���C���|�[�g�pPython�X�N���v�g
	Python\3dcg_tmo_export.py      tso�t�@�C���G�N�X�|�[�g�pPython�X�N���v�g
	Python\3dcg_armaturemimic.py   Armature��^��������Python�p�X�N���v�g
	Python\3dcg_weightmirror.py    3DCG�p�̃E�F�C�g�~���[Python�X�N���v�g
	Python\tdcg_change_mirror_bone_name.py	���E�Ώ̂̃E�F�C�g�ҏW�⏕�X�N���v�g
	
	readme.txt                     ���̃t�@�C��
	readme.html                    �ȒP�ȃ`���[�g���A��
	html(�t�H���_)                 readme.html �̃f�[�^��
	
	Sample.blend                   ���[�V����+���M���O�̃T���v��


���������@

Blender�̃X�N���v�g�t�H���_�Ɋg���q .py �̃t�@�C�����R�s�[���ĉ������B
��    C:\Program Files\Blender Foundation\Blender\.blender\scripts   ��...


���ȒP�Ȏg����

�Etso�t�@�C���̃C���|�[�g
Blender�̃��j���[�o�[���� File �� Import �� 3DCG tso file (.tso)... 
�ƑI������Ɛݒ����͂���ׂ�GUI���\�������̂ŁA��荞�ރf�[�^�̎�ނ�I���A
tso�t�@�C���̏ꏊ��I�ш�ԉ���Import�{�^�����N���b�N����Ǝ�荞�܂�܂��B

�Etso�t�@�C���̃G�N�X�|�[�g
Blender�̃��j���[�o�[���� File �� Export �� 3DCG tso file (.tso)... 
�ƑI������Ɛݒ����͂���ׂ�GUI���\�������̂ŁA�S�Ă̐ݒ���I���Ă���
�E����Export�{�^�����N���b�N�A�o�͐��ݒ肵������xExport�{�^�����N���b�N
�����tso�t�@�C�����o�͂ł��܂��B

�Etmo�t�@�C���̃C���|�[�g
Blender�̃��j���[�o�[���� File �� Import �� 3DCG tmo file (.tmo)... 
�ƑI������Ɛݒ����͂���ׂ�GUI���\�������̂ŁA�uTMO file select�v����
�Q��TMO�t�@�C����I�сuTMO Load�v�������ƃ{�^�����ǉ��ŕ\�������̂ŁA
�t���[���ԍ���I�у|�[�Y��K�p����Armature��I�����Ă���uPose Apply�v
�������ƃ|�[�Y���K�p����܂��B

�Etmo�t�@�C���̃G�N�X�|�[�g
Blender�̃��j���[�o�[���� File �� Export �� 3DCG tmo file (.tmo)... 
�ƑI������Ɛݒ����͂���ׂ�GUI���\�������̂ŁAArmature�I�u�W�F�N�g��I����
�o�͐�A�m�[�h�̎Q�l���I�񂾌�AExport�{�^�����N���b�N�����tmo�t�@�C����
�o�͂ł��܂��B

�EArmature Mimic
���Armature��I�����N��������ƁA�Ō�ɑI������Armature���ŏ��ɑI������
Armature�̓�����^��������B

�E3DCG�p �E�F�C�g�~���[
���b�V���I�u�W�F�N�g��I�����N������Ɛݒ��ʂ��\�������̂ŁA
�ǂ��炩��ǂ���ɒ��_�O���[�v���R�s�[�����邩�A�������l�A
���E�Ώ̃{�[���ƒ����{�[���̒��_�O���[�v�����ꂼ��ύX���邩�ǂ�����ݒ肵�AOK�������B

�E���E�Ώ̂̃E�F�C�g�ҏW�⏕�X�N���v�g
�I�u�W�F�N�g���[�h����X�N���v�g���N���ł��܂��B(3DCG Change mirror bone name)
���b�V���I�u�W�F�N�g���A�[�}�`���A�I�u�W�F�N�g��I��(�����I����)���A
�ϊ����[�h��I������Εϊ��ł��Ă���͂��ł��B
��̓I�ɂ́A�Ⴆ�΁ushiri_Right01�v�Ɓushiri_Left01�v���ushiri_01.R�v�Ɓushiri_01.L�v��
�ϊ�����āABlender��ō��E�Ώ̂̃{�[��(�E�F�C�g)�ƔF�������̂ŁA���ʕҏW���ȒP�ɂȂ�܂��B
���݃J�X�q�̃m�[�h�݂̂̑Ή��ł��B

�����ӎ���
Blender 2.49b�APython2.6�œ���m�F���Ă��܂��B


���ύX����

0.1 ����
0.2 3dcg_tso_import ���b�V���ǂݍ��ݕ�����UV�E�@���̃o�O�A���W�X�g���t�@�C���������ǂݎ��Ȃ��o�O���C��
0.21 tdcg_change_mirror_bone_name.py��ǉ�
