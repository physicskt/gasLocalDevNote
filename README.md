# gasLocalDevNote

## Google�A�J�E���g��clasp�Ƀ��O�C��
���̃R�}���h�����s���āAGoogle�A�J�E���g��clasp�Ƀ��O�C�����܂��B
```
clasp login
```

## PJ�̃t�H���_�Ɉړ�

## �悭�g�� clasp �R�}���h�܂Ƃ�
| �R�}���h                                   | ����                                               |
|--------------------------------------------|----------------------------------------------------|
| `clasp login`                              | Google�A�J�E���g�Ń��O�C��                         |
| `clasp logout`                             | ���O�A�E�g                                          |
| `clasp create --title "�^�C�g��"`           | �V����GAS�v���W�F�N�g���쐬                        |
| `clasp clone {�X�N���v�gID}`                | �����v���W�F�N�g���N���[��                          |
| `clasp push`                               | ���[�J���̕ύX��GAS�ɃA�b�v���[�h                   |
| `clasp pull`                               | GAS���̍ŐV�R�[�h���擾                             |
| `clasp open`                               | GAS��Web UI���u���E�U�ŊJ��                         |
| `clasp deployments`                        | �f�v���C�ς݈ꗗ���m�F                              |
| `clasp deploy --description "����"`         | �V�o�[�W�������쐬���ăf�v���C                      |
| `clasp version`                            | �o�[�W���������쐬�i�f�v���C�Ȃ��j                  |
| `clasp undeploy {�f�v���CID}`               | �f�v���C������                                      |
| `clasp list`                               | ���L���Ă���v���W�F�N�g�ꗗ��\��                   |
| `clasp status`                             | ���[�J����GAS�̍������m�F                           |
| `clasp logs`                               | ���s���O��\��                                      |
| `clasp run {�֐���}`                        | �w�肵���֐������s                                  |

## GAS�v���W�F�N�g�̃N���[��
�����̃v���W�F�N�g��ҏW����ꍇ�́A�v���W�F�N�g�̃X�N���v�gID���g�p���ăN���[�����܂��B
�X�N���v�gID�́AApps Script�G�f�B�^�́u�v���W�F�N�g�ݒ�v����m�F�ł��܂��B
```
clasp clone {�X�N���v�gID}
```

## �ύX�̃v�b�V��
�X�N���v�g�ɉ������ύX��Google Apps Script�ɔ��f������ɂ́A�ȉ��̃R�}���h���g�p���܂��B
```
clasp push
```

## ����f�v���C�i�o�[�W�����쐬 + �f�v���C�j
```
clasp deploy --description "����f�v���C"
```

## 2��ڈȍ~�̍X�V�i�ăf�v���C�j
```
clasp deploy --description "�C�����e�̐���"
```
```
clasp deploy --description "v1"  # �f�v���C���ăo�[�W�����쐬
```

## ���JURL�̊m�F�iWeb�A�v���̏ꍇ�j
```
clasp deployments
```
