# System-Threat-Forecaster
The goal of this competition is to predict a system’s probability of getting infected by various families of malware based on its configuration and usage properties.4

[![Kaggle](https://img.shields.io/badge/Kaggle-Competition-blue)]([https://www.kaggle.com/competitions/your-competition-name](https://www.kaggle.com/competitions/System-Threat-Forecaster/overview))


System Threat Forecaster

Can You Forewarn a System Before It’s Compromised?

# Description

The goal of this competition is to predict a system’s probability of getting infected by various families of malware based on its configuration and usage properties.

The dataset consists of telemetry data generated from threat reports collected by a system’s antivirus software. Using this data, participants must identify whether malware is detected on a given machine.

# Evaluation

Submissions are evaluated using the Accuracy Score (accuracy_score) between the predicted classes and the true target labels.

Submission File

For each id in the test set, you must predict a class value for the target variable.

Submission Format
| id | target |
| -- | ------ |
| 0  | 0      |
| 1  | 1      |
| 2  | 1      |
| 4  | 0      |
| 5  | 1      |
| …  | …      |


Each row in the dataset corresponds to a unique machine, identified by MachineID.

target indicates whether malware was detected on the machine.

Using the information in train.csv, participants must predict target for each machine in test.csv.

Files

train.csv — Training dataset with features and target labels

test.csv — Test dataset without target labels

sample_submission.csv — Example submission file in the correct format

# Columns

Identifiers

MachineID — Unique identifier for each machine

Antivirus & Security Configuration

ProductName — Installed antivirus product

EngineVersion — Antivirus engine version

AppVersion — Antivirus application version

SignatureVersion — Malware signature version

IsBetaUser — Whether the user is on a beta version

RealTimeProtectionState — Real-time protection status

IsPassiveModeEnabled — Passive mode enabled or not

AntivirusConfigID — Antivirus configuration identifier

NumAntivirusProductsInstalled — Number of installed antivirus products

NumAntivirusProductsEnabled — Number of enabled antivirus products

IsSystemProtected — System protection status

FirewallEnabled — Windows firewall status

EnableLUA — User Account Control enabled

AutoSampleSubmissionEnabled — Auto sample submission setting

Hardware & Device Information

HasTpm — Trusted Platform Module presence

Processor, ProcessorCoreCount, ProcessorModelID, ProcessorManufacturerID

TotalPhysicalRAMMB

PrimaryDiskCapacityMB, SystemVolumeCapacityMB

PrimaryDiskType

HasOpticalDiskDrive

ChassisType

DeviceFamily

OEMNameID, OEMModelID

PowerPlatformRole

InternalBatteryNumberOfCharges

IsVirtualDevice

IsPortableOS

IsTouchEnabled, IsPenCapable

IsAlwaysOnAlwaysConnectedCapable

IsGamer

Operating System Information

OSVersion

OSBuildNumber, OSBuildLab

OSBuildNumberOnly, OSBuildRevisionOnly

OSProductSuite

OsPlatformSubRelease

OSArchitecture

OSBranch

OSEdition

OSSkuFriendlyName

OSInstallType

OSInstallLanguageID

OSUILocaleID

NumericOSVersion

OSGenuineState

LicenseActivationChannel

SMode

Browser & Interface

IEVersionID

Geographic Information

CountryID

CityID

GeoRegionID

LocaleEnglishNameID

RegionIdentifier

Update & Firmware Information

AutoUpdateOptionsName

IsFlightsDisabled

FlightRing

FirmwareManufacturerID

FirmwareVersionID

IsSecureBootEnabled

Dates

DateAS — Malware signature date

DateOS — Timestamp of last OS update

Target Variable

target — Indicates whether malware was detected on the machine (0 = No, 1 = Yes)
